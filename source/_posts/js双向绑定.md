---
title: js双向绑定
date: 2018-12-04 17:19:54
tags: 技术

---

## 前端数据双向绑定的方法

​	最近在维护一个项目是用的jQuery写的，但是因项目需求我用到了双向绑定来解决问题，现在记录一下原生js的双向绑定的几种方法

----

---

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title></title>
</head>
<body>
<input type="text" id="aa"/>
<span id="bb">{{hello}}</span>
<script>
    var obj = {};
    Object.defineProperty(obj,'hello',{
        set:function(val){
            document.getElementById('bb').innerHTML = val;
            document.getElementById('aa').value = val;
        }
    });
    document.getElementById('aa').onkeyup = function(e){
        obj.hello = e.target.value;
    };
    obj.hello = "hello world!";


</script>
</body>
</html>
```

上边是一个简单的例子 前端数据劫持完成，使用define Property,(代表Vue js)

<!--more-->







```html
	<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>原生js实现数据双向绑定</title>

</head>
<body>
<!--这里是html内容-->
<h1>原生js双向绑定及其应用</h1>
<div class="js-2-1section2 col-sm-10 col-xs-10">
    <div><input type="text" data-bind-1="peopleName"  id="text1"/>
        <!--data-bind-1="peopleName" 原生js双向绑定的格式-->
    </div>
    <div><input  type="text" data-bind-2="killName" id="text2" />
    </div>
    <div><input  type="text" data-bind-3="killName1" id="text3" />
    </div>
    <p data-bind-1="peopleName"></p>
    <p data-bind-2="killName"></p>
    <p data-bind-3="killName1"></p>
    <!--<p>手动输入框里面值的获取DBind1.attributes.peopleName</p>-->
</div>
<!--下面这部分是生成原生js的代码-->
<script>
    var DBind1 = new DBind( 1 );
    var DBind2 = new DBind( 2 );//前面是变量，括号里面的是html那里填的数字
    var DBind3 = new DBind( 3 );//前面是变量，括号里面的是html那里填的数字
    DBind1.set( "peopleName", '第一个' );
    DBind2.set( "killName", '第二个' );//第一个是刚才html格式那里的变量名，第二个方框是赋值
    DBind3.set( "killName1", '第san个' );
    function DataBinder( object_id ) {
        // 创建一个简单的pubSub对象
        var pubSub = {
                    callbacks: {},

                    on: function( msg, callback ) {
                        this.callbacks[ msg ] = this.callbacks[ msg ] || [];
                        this.callbacks[ msg ].push( callback );
                    },

                    publish: function( msg ) {
                        this.callbacks[ msg ] = this.callbacks[ msg ] || [];
                        for ( var i = 0, len = this.callbacks[ msg ].length; i < len; i++ ) {
                            this.callbacks[ msg ][ i ].apply( this, arguments );
                        }
                    }
                },

                data_attr = "data-bind-" + object_id,
                message = object_id + ":input",
                timeIn;

        changeHandler = function( evt ) {
            var target = evt.target || evt.srcElement, //  IE8兼容
                    prop_name = target.getAttribute( data_attr );

            if ( prop_name && prop_name !== "" ) {
                clearTimeout(timeIn);
                timeIn = setTimeout(function(){
                    pubSub.publish( message, prop_name, target.value );
                },50);

            }
        };

        // 监听事件变化，并代理到pubSub
        if ( document.addEventListener ) {
            document.addEventListener( "input", changeHandler, false );
        } else {
            // IE8使用attachEvent而不是addEventListenter
            document.attachEvent( "oninput", changeHandler );
        }

        // pubSub将变化传播到所有绑定元素
        pubSub.on( message, function( evt, prop_name, new_val ) {
            var elements = document.querySelectorAll("[" + data_attr + "=" + prop_name + "]"),
                    tag_name;

            for ( var i = 0, len = elements.length; i < len; i++ ) {
                tag_name = elements[ i ].tagName.toLowerCase();

                if ( tag_name === "input" || tag_name === "textarea" || tag_name === "select" ) {
                    elements[ i ].value = new_val;
                } else {
                    elements[ i ].innerHTML = new_val;
                }
            }
        });

        return pubSub;
    }
    function DBind( uid ) {
        var binder = new DataBinder( uid ),

                user = {
                    // 属性设置器使用数据绑定器pubSub来发布
                    attributes: {},
                    set: function( attr_name, val ) {
                        this.attributes[ attr_name ] = val;
                        // Use the `publish` method
                        binder.publish( uid + ":input", attr_name, val, this );
                    },
                    get: function( attr_name ) {
                        return this.attributes[ attr_name ];
                    },

                    _binder: binder
                };

        // Subscribe to the PubSub
        binder.on( uid + ":input", function( evt, attr_name, new_val, initiator ) {
            if ( initiator !== user ) {
                user.set( attr_name, new_val );
            }
        });

        return user;
    }
</script>


<!--这里是原生js双向绑定的应用。-->

</body>
</html>
```

这个是封装比较完善的一个

**上面代码中data-bind-1=”peopleName” 比较重要，其他一些乱七八糟，用来实现效果的，可以不用管。**