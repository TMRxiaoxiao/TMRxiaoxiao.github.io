---
title: hexo相关
date: 2018-11-21 16:54:08
tags: 随笔
---

````
<!DOCTYPE html>
<html>

<head>
	<meta charset="UTF-8">
	<title>个人定制</title>
	<meta name="viewport" content="width=1300">


	<!-- Le styles -->
	<link type="text/css" rel="stylesheet" href="mycode/css/jquery.miniColors.css" />

	<link rel="stylesheet" type="text/css" href="css/cssreset.css" />
	<link rel="stylesheet" type="text/css" href="css/customization.css" />
	<link rel="stylesheet" type="text/css" href="css/two.css" />
	<link rel="stylesheet" type="text/css" href="css/selectFilter.css" />

</head>
````
<!--more-->
````
<style>
	.cover {
		    height: 100%;
		}
	.cover .fill-info {
	    height: 670px;
	    position: fixed;
	}
	.cover .fill-info {
    width: 725px;
		}
	.cover .table-box {
    width:576px;
    margin: 0 auto;
    overflow: hidden;
    height: 350px;;
    overflow-y: auto;
	}
	.cover .table-box::-webkit-scrollbar {
        display: none;
    }
	.cover table {
    width: 566px;
    border: 1px solid #eee;
    font-size: 13px;
	}
	.cover .fill-info .top-title {
    height: 60px;
    line-height: 60px;
	}
	.cover-ul {
    overflow: hidden;
    padding-top: 25px;
    box-sizing: border-box;
    padding-left: 46px;
	}
	.cover .cover-ul li {
    overflow: hidden;
    padding-left: 30px;
    margin-bottom: 10px;
	}
	.cover .spanbox {
  	margin-top: 5px;
	}
	.cover .fill-info .top-title .x-button {
    margin-top: 17px;
    margin-right: 22px;
    cursor: pointer;
}
	.cover .fill-info .top-title span {
	    margin-left: 40px;
	}
	.sucai button {
    display: block;
    width: 238px;
    height: 50px;
    border: none;
    background: #FF6700;
    border-radius: 3px;
    margin: 24px auto 0 auto;
    color: white;
    font-size: 15px;
}
.cover .table-left {
    text-align: center;
     padding-left: 0px; 
}
	.suremake {
  	position: absolute;
    bottom: -157px;
	cursor:pointer;
    left: 272px;
}
	.cover-content{
		position: relative;
	}
	.change{
		background: #FF6700;
	}
	.namework{
		width: 420px;
	    height: 37px;
	    background: #f0f4f9;
	    color: black;
	    outline: none;
	    border: none;
	    padding: 10px;
	    margin-bottom: 20px;
	    margin-top: 30px;
	}
	.textwork{
		width: 420px;
	    height: 100px;
	    background: #f0f4f9;
	    color: black;
	    outline: none;
	    border: none;
	    padding: 10px;
	    resize: none;
	}
	.selltitle>span {
    width: 49%;
}
	.sellcontent {
    padding: 0 78px;
}
	.post div select {
    width: 359px;
}
	.mains-left .left-size {
		width: 100%;
		height: 73px;
		box-sizing: border-box;
		padding: 0 15px;
		/* background: yellow; */
	}
	.mains-left .left-size p {
		height: 20px;
		line-height: 20px;
		font-size: 15px;
		margin-top: 27px;
		margin-bottom: 15px;
	}
	.mains-left .left-size ul {
		width: 100%;
		height: 36px;
		display: flex;
		justify-content: flex-start;
		flex-wrap: wrap;
		align-items: center;
	}
	.mains-left .left-size li {
		width: 24%;
		box-sizing: border-box;
		text-align: center;
		/* vertical-align: middle; */
		height: 38px;
		line-height: 38px;
		margin-right: 1%;
		background: #f0f4f9;
		cursor: pointer;
		margin-bottom: 10px;
	}
	.click {
		background: #fff!important;
		border: 1px solid #FF6700!important;
		box-sizing: border-box!important;
		color: #FF6700!important;
	}
	//  
	.change_img {
		width: 140px;
		height: 37px;
	}
	.change_img > div {
		width: 70px;
		height: 100%;
		color: #9c9c9d;
		background: #ffffff;
		float: left;
		text-align: center;
		line-height: 37px;
		font-size: 14px;
		cursor: pointer;
	}
	.change_img > div.selected{
		background: #a2a9b2;
		color: #e1e3e6;
	}
	/*  */
	#design-img {
		display: block;
		position: absolute;
	}
	</style>

<body>
	<div id="head"></div>
	<div class="direct-bar">
		<ul class="direct-bar-ul">
			<li><span>首页</span></li>
			<li><span>商城</span></li>
			<li><span>团体定制</span></li>
			<li><span class="dh-current">个人定制</span></li>
			<li><span>众筹</span></li>
		</ul>
	</div>
	<div id="main">
		<div class="doc" style="width: 1340px;position: relative;overflow: inherit;">
			<!-- title -->
			<div class="title">
				<div class="title-left">
					<span class="indexs">1</span>
					<span class="indexss">在线设计我的作品</span>
				</div>
				<div class="title-right">
					<span class="indexs2">2</span>
					<span class="indexss2">在线购买/出售作品</span>
				</div>
			</div>
			<div class="mains-left" id="mains-left">
				<div class="makeworks">
					<div class="left-top" id="left-top">

					</div>
					<div class="left-style" id="left-style">

					</div>
					<div class="left-size" id="left-size">

					</div>
					<div class="left-color" id="left-color">

					</div>
				</div>
				<div class="sellworks" style="display: none">
					<p class="worknews">作品信息</p>
					<p class="workname">作品名称</p>
					<input type="text" placeholder="请想个标题哦~" value="" class="namework">
					<p class="workdescrible">作品描述</p>
					<textarea name="" placeholder="添加我的描述" class="textwork"></textarea>
				</div>

			</div>
			<!-- 设计效果图 -->
			<div class="main-center">
				<div class="change_img">
					<div class="design selected" data-id="0">设计图</div>
					<div class="effect" data-id='1'>效果图</div>
				</div>
				<div data-id='0' id="design-center" class="img-center-toggle">
					<div id="shirtDiv" class="page" style="width: 464px; height: 464px; position: relative; background-color: rgb(255, 255, 255); margin-top: 47px; margin-bottom: 20px;">
						<div id="drawingArea" style="position: absolute;top: 50px;left:50px;z-index: 10;width: 414px;height: 414px;">
							<canvas id="tcanvas" width=414 height="414" class="hover" style="-webkit-user-select: none;  border: 1px solid #e1e3e6"></canvas>
						</div>
					</div>
				</div>
				<div data-id='1' id="img-center" style="height: 464px; margin-bottom: 20px;" class="img-center-toggle">
					<div id="shirtDiv" class="page" style="width: 464px; height: 464px; position: relative; background-color: rgb(255, 255, 255); margin-top:47px; margin-bottom: 20px; clear:both;">
						<img id="tshirtFacing" src="" alt=" " style="width: 100%; height: 464px; display:none"></img>
						<!-- <div id="drawingArea" style="position: absolute;top: 100px;left:142px;z-index: 10;width: 180px;height: 350px;">
							<canvas id="tcanvas" width=180 height="350" class="hover" style="-webkit-user-select: none;"></canvas>
						</div> -->
						<!-- <img id="design-img" src="data:image/png;base64," alt=""> -->
						<img id="design-img" src="" alt="">
					</div>
				</div>
				<div style="text-align:center; position:absolute; left:0; bottom:107px; width:100%; display:none" id="opslider">
					<input id="snrPollInterval" type="range" value="100"></div>
				<div id="btn-center">
					<span class="active zhengimg" data-type="a" data-img1=''>正面</span>
					<span data-type="b" data-img2='' class="fanimg">反面</span>

				</div>
				<div class="set" id='setClick'>
					<span><img src="img/icons/icon1.png" id="remove-selected"></span>
					<span><img src="img/icons/icon2.png" data-click='Copy' ></span>
					<span><img src="img/icons/icon3.png" data-click='flipX' ></span>
					<span><img src="img/icons/icon4.png" data-click='flipY' ></span>

				</div>
			</div>
			<div class="main-right">
				<!-- <input type="text" name="" id="title" value="" placeholder="作品标题" />
	    			<textarea name="" rows="" cols="" id="describe" placeholder="请在此输入作品描述"></textarea>
	    			<input type="button" name="" id="buy" value="下单购买" />
	    			<input type="button" name="" id="sell" value="发起售卖" /> -->
				<div class="makesright">
					<div class="right-top">
						<span>图片</span>
						<span>素材库</span>
						<span>文字</span>
					</div>
					<div class="right-content">
						<div class="imgs content">
							<div class="img-title" style="margin:15px;  text-align:left">
								<span class="click-sucai">上传</span>
								<span class="">工具</span>

							</div>
							<div class="uplaodlayer">
								<div class="imgs-text">
									推荐使用格式为PNG格式</br>
									尺寸不小于150*150px的透明背景图片</br>
									避免线条过细</br>
									可以通过拖拽图片调整位置和大小</br>
								</div>
								<div class="imgs-up">
									<input type="button" id="upload" value="上传图片" />
									<input type="file" name="" id="file" value="" style="display:none" />
								</div>
								<ul class="img-content">


								</ul>
							</div>

							<div class="toolslayer" style="display:none; padding:15px;">
								<div style="text-align:left"> 图形吸附工具</div>
								<ul class="tools-imgs" id='picture-tool'>
									<li><img src="img/tools_1.png" class="img-tools"></li>
									<li><img src="img/tools_2.png" class="img-tools" data-click='loadPattern'></li>
									<li><img src="img/tools_3.png" class="img-tools" data-click='loadPattern4'></li>
									<li><img src="img/tools_4.png" class="img-tools" data-click='loadPattern3'></li>
									<li><img src="img/tools_5.png" class="img-tools" data-click='loadPattern5'></li>
									<li><img src="img/tools_6.png" class="img-tools" data-click='loadPattern2'></li>
									<li><img src="img/tools_7.png" alt="圆角矩形" class="img-tools" data-click='loadPatternRoundRect'></li>
									<li><img src="img/tools_8.png" alt="图形1" class="img-tools" data-click='loadPatternGraph1' ></li>
									<li><img src="img/tools_9.png" alt="图形2" class="img-tools" data-click='loadPatternGraph2' ></li>
									<li><img src="img/tools_10.png" alt="图形3" class="img-tools" data-click='loadPatternGraph3'></li>
									<li><img src="img/tools_11.png" alt="图形4" class="img-tools" data-click='loadPatternGraph4'></li>
									<li><img src="img/tools_12.png" alt="图形5" class="img-tools" data-click='loadPatternGraph5'></li>
									<li><img src="img/tools_13.png" alt="图形6" class="img-tools" data-click='loadPatternGraph6'></li>
									<li><img src="img/tools_14.png" alt="图形7" class="img-tools" data-click='loadPatternGraph7' ></li>

								</ul>
								<div style="text-align:left; margin-top:45px;"> 滤镜工具</div>
								<ul class="tools-imgs" id="filter-tool">
									<li data-click='' ><img src="img/tools_1.png" class="img-tools"></li>
									<li data-click='Grayscale'><img src="img/f_2.png" class="img-filter"></li>
									<li data-click='kodachrome' ><img src="img/f_1.png" class="img-filter"></li>
									<li data-click='Invert' ><img src="img/f_3.png" class="img-filter"></li>
									<li data-click='technicolor' ><img src="img/f_4.png" class="img-filter"></li>

								</ul>


							</div>

							<!--<label>滤镜:
                                  <select id="filter-selector" name="filters">
                                      <option selected="" value="add">选择滤镜</option>
                                      <option value="vintagePinhole">Vintage Pinhole</option>
                                      <option value="kodachrome">Kodachrome</option>
                                      <option value="technicolor">Technicolor</option>
                                  </select>
                              </label>-->
							<button class="next-walk">下一步</button>
						</div>
						<div class="sucai content" id="sucai">

						</div>
						<div class="text content">
							<textarea name="" id="text-string" cols="30" rows="10" placeholder="请在此输入作品描述"></textarea>
							<div>
								<p>
									<span>字体</span>
									<select name="" id="font-family">
										<option value="微软雅黑">微软雅黑</option>
										<option value="宋体">宋体</option>
										<option value="MuyaoSoftbrush">MuyaoSoftbrush</option>
										<option value="fzqtfw">fzqtfw</option>
										<option value="fzsejw">fzsejw</option>
										<option value="HYShangWeiLiuYunTiJ-2">HYShangWeiLiuYunTiJ-2</option>
										<option value="方正明尚简体">方正明尚简体</option>
										<option value="方正清刻本悦宋简体">方正清刻本悦宋简体</option>
										<option value="方正特粗光辉简体">方正特粗光辉简体</option>
										<option value="方正特雅宋体">方正特雅宋体</option>
										<option value="方正字迹-佛君包装简体">方正字迹-佛君包装简体</option>
										<option value="海派腔调禅大黑简2.0">海派腔调禅大黑简2.0</option>
										<option value="海派腔调奶油简">海派腔调奶油简</option>
										<option value="汉仪程行简">汉仪程行简</option>
										<option value="汉仪蝶语体简">汉仪蝶语体简</option>
										<option value="汉仪立黑简">汉仪立黑简</option>
										<option value="汉仪双线体简">汉仪双线体简</option>
										<option value="锐字工房光芒黑简1.0">锐字工房光芒黑简1.0</option>
									</select>
								</p>
								<p>
									<span>填充</span>
									<span style="margin-left:15px;"><input type="hidden" id="text-fontcolor" class="color-picker" size="7" value="#000000"></span>
								</p>
								<p>
									<span>描边</span>
									<span style="margin-left:15px;"><input type="hidden" id="text-strokecolor" class="color-picker" size="7" value="#000000"></span>
								</p>

								<p>
									<span>样式</span>
									<span style="margin-left:15px;"><img id="text-bold" src="mycode/img/font_bold.png" height="" width="" style="vertical-align: middle;"></span>
									<span style="margin-left:15px;"><img id="text-italic" src="mycode/img/font_italic.png" height="" width=""
										 style="vertical-align: middle;"></span>
									<span style="margin-left:15px;"><img id="text-strike" src="mycode/img/font_strikethrough.png" height="" width=""
										 style="vertical-align: middle;"></span>
									<span style="margin-left:15px;"><img id="text-underline" src="mycode/img/font_underline.png" height="" width=""
										 style="vertical-align: middle;"></span>
								</p>
								<p><button id="add-text">
										加入文字
									</button></p>

							</div>
							<button class="next-walk">
								下一步
							</button>

						</div>
					</div>
				</div>
				<div class="sellright" style="display: none;">
					<div class="selltitle">
						<span>我要购买</span>
						<span>我要出售</span>
					</div>
					<div class="buywork">
						<div class="sellcontent">
							<div class="sell-buy">
								<p>
									<span class="dingzhi">定制</span>
									<span class="sheji sheji1">商品定制</span>
								</p>
								<p class="miaoshu miaoshu1">

								</p>
								<p>
									<span class="money">价格 <i></i></span>
								</p>
								<!-- 虚线框 -->
								<div class="dz" id="dz">
									<ul class="dz-ul">
										<li>
											<img src="img/orange-circle-tick.gif" alt="">
											<span id="bqx">个人版权</span>
										</li>

									</ul>
								</div>
								<div class="yixuan">
									<span>已选</span>
									<span class="yixuancont">短T/男装/白色</span>
								</div>
								<div class="chima" id='chima'>
									<span>尺码</span>
									<ul>
										<li class="click"></li>
									</ul>

								</div>
								<div class="number-div">
									<span>数量</span>
									<div class="add-num-div">
										<i class="product-num">1</i>
										<div class="add-button-div">
											<ul class="adddel-ul">
												<li class="addbtn">+</li>
												<li class="delbtn">–</li>
											</ul>
										</div>
									</div>
									<span id="kucun"></span>
								</div>

							</div>
						</div>

						<div class="sellbottom">
							<button class="cart backp">

								<span>返回上一步</span>
							</button>
							<button class="buys comebuy">立即购买</button>
						</div>
					</div>
					<div class="sellwork" style="display: none">
						<div class="sellcontent">
							<div class="sell-sell">
								<!-- <p>
				    					<span class="dingzhi">定制</span>
				    					<span class="sheji">商品定制</span>
				    				</p> -->
								<div class="miaoshu">
									<input type="text" placeholder="我的作品叫什么？" class="namework" id="namework">
									<textarea name="" placeholder="添加我的描述" class="textwork" id="textwork"></textarea>
								</div>
								<!-- 虚线下面内容-->
								<div class="post">
									<!--	<div class="peisong">
				    						<span>配送</span>
				    						<select name="" id="post-way">
					    						<option value="">特快：加15元升级为顺丰</option>
					    						<option value="">卡通2</option>
					    						<option value="">卡通3</option>
					    						<option value="">卡通4</option>
					    					</select>
				    					</div>-->
									<!--<span>为买家选择配送方式，该该费用由设计师为买家承担</span>-->
									<div class="banquan">
										<span>版权</span>
										<select name="" id="banquan">

										</select>
									</div>
								</div>
							</div>

						</div>

						<div class="sellbottom">
							<button class="cart carts">
								<img src="" alt="">
								<span>设置售卖价格</span>
							</button>
							<button class="buys fabu">立即发布</button>
						</div>
					</div>
				</div>
			</div>
		</div>
		<div id="foot"></div>
		<!--发起售卖弹出框-->
		<div class="cover">
			<div class="fill-info">
				<div class="top-title">
					<span>设置售卖价格</span>
					<img src="img/x-button.gif" alt="" class="x-button" />
				</div>
				<div class="cover-content">
					<ul class="cover-ul">
						<li>
							<span class="cu-name">一键设置产品图案费用</span>
							<div class="inputbox">
								<span>&yen;</span><input type="text" placeholder="请输入产品图案价格" onkeyup="value=value.replace(/[^\d]/g,'') " value=""
								 size="4" maxlength="4" onbeforepaste="clipboardData.setData('text',clipboardData.getData('text').replace(/[^\d]/g,''))" />
							</div>
						</li>
					</ul>
					<div class="table-box">
						<table border="0" cellspacing="0" cellpadding="0" id="trs">
							<tr>
								<th class="table-left" style="width: 70px;border-bottom: 1px solid #eee;">服装</th>
								<th class="table-left" style="width: 70px;border-bottom: 1px solid #eee;">款式</th>
								<th class="table-left" style="width: 70px;border-bottom: 1px solid #eee;">颜色</th>
								<th class="table-left" style="width: 70px;border-bottom: 1px solid #eee;">尺码</th>
								<th style="width: 90px;border-bottom: 1px solid #eee;">原价</th>
								<th style="border-bottom: 1px solid #eee;">一键设置产品售价</th>
								<th style="width: 90px;border-bottom: 1px solid #eee;">单件利润</th>
							</tr>
						</table>
					</div>
					<button class="suremake">确认设置</button>
				</div>
			</div>
		</div>
		<!-- 商品属性左边 -->
		<script id="left-top-template" type="text/x-dot-template">
			<div class="filter-box">
		<div class="filter-text">
			<input class="filter-title" type="text" readonly placeholder="选择服装" />
			<i class="icon icon-filter-arrow"></i>
		</div>
		<select name="filter">

			{{ for(var i in it) { }}
           		<option data-id="{{=it[i].id}}" data-img="{{=it[i].imageurl}}">{{=it[i].typename}}</option>
            {{ } }}
		</select>
	    </div>
			

		</script>
		<script id="left-style-template" type="text/x-dot-template">
			<p>款式</p>
		  	<ul>
		  		{{ for(var i in it) { }}
           		<li data-id="{{=it[i].clothingid}}">{{=it[i].clothingname}}</li>
            	{{ } }}
		  	</ul>
		</script>
		<script id="left-size-template" type="text/x-dot-template">
			<p>尺码</p>
		  	<ul>
		  		{{ for(var i in it) { }}
           		<li data-id="{{=it[i].sizeid}}" data-moneys="{{=it[i].moneys}}" data-numbers="{{=it[i].numbers}}" >{{=it[i].sizename}}</li>
            	{{ } }}
		  	</ul>
		</script>
		<script id="left-color-template" type="text/x-dot-template">
			<p>颜色</p>
		
		  	<ul>
		  		{{ for(var i in it) { }}
				  <li class="color-preview " title="{{=it[i].colorname}}" data-color="#ffffff" data-id="{{=it[i].id}}" data-img1="{{=it[i].imageurlup}}" data-img2="{{=it[i].imageurldown}}"><img src="{{=it[i].imageurlup}}" alt=""></li>
            	{{ } }}
		  	</ul>
		</script>
		<!-- 素材库 -->
		<script id="sucai-template" type="text/x-dot-template">
			<div class="sucai-title">
				<span>推荐</span>
				<span>搭配</span>
				<span>背景</span>
			</div>
			<select name="" id="select-sucai">
				{{ for(var i in it.list) { }}
           			<option value="{{=it.list[i].id}}">{{=it.list[i].nickname}}</option>
            	{{ } }}
			</select>
			<ul class="sucai-imgs">
				{{ for(var i in it.list[0].detaillist) { }}
           			<li><img src="{{=it.list[0].detaillist[i].imageurl}}" class="img-polaroid"></li>
            	{{ } }}
			</ul>
			<button class="next-walk">下一步</button>
		</script>
		<!-- 商品属性 -->
		<!-- <script id="dz-template" type="text/x-dot-template">
		  	<ul class="dz-ul">
		  		{{ for(var i in it) { }}
           			<li>
					<img src="img/orange-circle-tick.gif" alt="">{{=it[i].Attributename}}
					</li>
            	{{ } }}
		  	</ul>
		</script> -->
		<!-- 商品尺码 -->
		<script id="chima-template" type="text/x-dot-template">
			<span>尺码</span>
				<ul>
					{{ for(var i in it) { }}
	           			<li data-money="{{=it[i].moneys}}" data-num="{{=it[i].numbers}}" data-sizeid="{{=it[i].sizeid}}" data-id="{{=it[i].id}}">{{=it[i].sizename}}</li>
	            	{{ } }}
				</ul>
		</script>
		<!-- 版权 -->
		<script id="banquan-template" type="text/x-dot-template">
			{{ for(var i in it) { }}
	           			<option value="{{=it[i].id}}">{{=it[i].servicename}}</option>
	            	{{ } }}
		</script>
		<script src="js/jquery-1.11.3.js" charset="utf-8"></script>
		<script src="mycode/js/html2canvas.js"></script>
		<script src="mycode/js/fabric.js"></script>
		<script src="mycode/js/colorMatrixFilter.js"></script>
		<script src="mycode/js/tshirtEditor.js"></script>
		<script src="mycode/js/customiseControls.js"></script>
		<script src="mycode/js/fontfaceobserver.js"></script>
		<script src="mycode/js/jquery.miniColors.min.js"></script>
		<script src="js/jquery.cookie.js"></script>
		<script src="js/load-head-foot.js"></script>
		<script src="js/common.js"></script>
		<script src="js/doT.min.js"></script>
		<script src="js/selectFilter.js"></script>
		<script>
			//  个人定制点击设计图和效果图切换
			$(function () {
				function desginImg(w, h, l, t, s) {
					$('#design-img').css({
						width: w + 'px',
						height: h + 'px',
						left: l + 'px',
						top: t + 'px',
					})
					$('#design-img').attr('src', s)
				}
				
				if ($('.change_img > .design').hasClass('selected')) {
					$('#design-center').show()
					$('#img-center').hide()
				} else {
					$('#design-center').hide()
					$('#img-center').show()
				}
				$('.change_img').on('click', 'div', function () {
					$('.change_img').find('div').removeClass('selected')
					$('.img-center-toggle').hide()
					var dataId = $(this).attr('data-id')
					$(this).addClass('selected')
					$('.img-center-toggle').each((index, val) => {
						if (dataId == index) {
							$(val).show()
						}
					})
					if(dataId == 1) {
						$("#opslider").css('display', 'none');
					} else {
						if(localStorage.sliderStatus == 'true') {
							$("#opslider").css('display', 'block');
						} else {
							$("#opslider").css('display', 'none');
						}
					}
				})

			})
		</script>
		<script>
			//点击title的时候颜色发生变化以及下面内容切换
			$(document).on('click', '.title-left', function () {
				var thisa = $(this)
				$.MsgBox({
					type: "confirm",
					speed: 200,
					title: "",
					msg: '确定重新设计吗？',
					opacity: '0.1',
					callback: function () {
						$(thisa).find('.indexs').css('background', '#FF6700')
						$(thisa).find('.indexss').css('color', '#FF6700')
						$(thisa).siblings().find('.indexs2').css('background', 'black')
						$(thisa).siblings().find('.indexss2').css('color', 'black')
						$('.makeworks').addClass('show').siblings().addClass('hide')
						$('.makesright').addClass('show').siblings().addClass('hide')
						$('.makeworks').removeClass('hide').siblings().removeClass('show')
						$('.makesright').removeClass('hide').siblings().removeClass('show')
						$('#mains-left').css('display', 'block')
						$('.main-center').css('width', '550px ')
						$('.main-right').css('width', '393px')
						$('#img-center').css('width', '464px')
						$('#img-center').css('margin-left', '42px')
						$('#shirtDiv').css('width', '464px')
						$('#btn-center').css('margin-left', '205px')
						$('.set').show()


						$('.change_img').show()
						$('.img-center-toggle').eq(0).show()
						$('.img-center-toggle').eq(1).hide()
						if(localStorage.sliderStatus == 'true') {
							$('#opslider').show()
						}
						$('.change_img').find('div').removeClass('selected')
						$('.design').addClass('selected')
						for (var i = 0; i < inumber; i++) {
							canvas.item(i).selectable = true;
						}
					}
				});

			})
			// $(document).on('click','.title-right',function(){
			// 	$(this).find('.indexs2').css('background','#FF6700')
			// 	$(this).find('.indexss2').css('color','#FF6700')
			// 	$(this).siblings().find('.indexs').css('background','black')
			// 	$(this).siblings().find('.indexss').css('color','black')
			// 	$('.sellworks').addClass('show').siblings().addClass('hide')
			// 	$('.sellright').addClass('show').siblings().addClass('hide')
			// 	$('.sellworks').removeClass('hide').siblings().removeClass('show')
			// 	$('.sellright').removeClass('hide').siblings().removeClass('show')
			// })
			//点击下一步的时候
			$(document).on('click', '.next-walk', function () {
				$('.change_img').hide()
				$('.img-center-toggle').eq(0).hide()
				$('.img-center-toggle').eq(1).show()
				$('#opslider').hide()
				var tid = GetQueryString('tid')
				var sid = GetQueryString('sid')
				var cid = GetQueryString('cid')

				if (tid && sid) {
					shopping(tid, sid, cid)
					tf = canvas.toDataURL('png').replace(/^.*?,/, '');


					$('.title-right').find('.indexs2').css('background', '#FF6700')
					$('.title-right').find('.indexss2').css('color', '#FF6700')
					$('.title-right').siblings().find('.indexs').css('background', 'black')
					$('.title-right').siblings().find('.indexss').css('color', 'black')
					$('.sellworks').addClass('show').siblings().addClass('hide')
					$('.sellright').addClass('show').siblings().addClass('hide')
					$('.sellworks').removeClass('hide').siblings().removeClass('show')
					$('.sellright').removeClass('hide').siblings().removeClass('show')
					$('#mains-left').css('display', 'none')
					//$('.main-center').css('width','757px')
					$('.main-right').css('width', '765px')
					//$('#img-center').css('width','600px')
					$('#img-center').css('margin-left', '52px')
					$('.set').hide()
					for (var i = 0; i < inumber; i++) {
						canvas.item(i).selectable = false;
					}
				} else {

					$.MsgBox({
						type: "alert",
						speed: 200,
						title: "",
						msg: '请选择完整的规格',
						opacity: '0.1',
					});
				}

				//$('#shirtDiv').css('width','600px')
				//$('#btn-center').css('margin-left','264px')
			})

			//点击定制需求填写弹出填写框
			$('.carts').on("click", function () {
				$('.cover').fadeIn();
			})
			//点击x关闭弹出框
			$('.x-button').on("click", function () {
				$('.cover').fadeOut();
			})
			$('.back').on("click", function () {
				$('.cover').fadeOut();
			})

			//购买出售商品切换
			$('.selltitle>span').eq(0).addClass('click-sell')
			$(document).on('click', '.selltitle span', function () {
				var sign = $(this).index()
				$(this).addClass('click-sell').siblings().removeClass('click-sell')
				if (sign == 0) {
					$('.buywork').css('display', 'block')
					$('.sellwork').css('display', 'none')
				} else {
					$('.buywork').css('display', 'none')
					$('.sellwork').css('display', 'block')
				}
			})

			//加减
			$('.add-num-div').on('click', '.addbtn', function () {
				var count = parseInt($('.product-num').html())
				var numbers = $('.left-size ul li.click').attr('data-numbers')
				if (count >= numbers) {
					return;
				}
				count++;
				$('.product-num').html(count);
				num = count;
			})
			$('.add-num-div').on('click', '.delbtn', function () {
				var count = parseInt($('.product-num').html())
				if (count <= 1) {
					return;
				}
				count--;
				$('.product-num').html(count);
				num = count;
			})

			//上传
			$("#upload").click(function () {
				$("#file").trigger("click");
			});
			$(document).on('change', '#file', function () {
				var file = this.files[0];
				if (!/image\/\w+/.test(file.type)) {
					alert("请确保文件为图像类型");
					return false;
				}
				var reader = new FileReader();
				reader.readAsDataURL(file);
				reader.onload = function () {

					var html = '<li><span><img class="remove" src="img/moveimgs.png" ></span><img class="img-polaroid" src="' +
						this.result + '" style="width: 100%;height: 100%;object-fit: cover;" ></li>'
					if ($('.img-content li').length < 4) {
						$('.img-content').append(html);
						// console.log($('.img-content li').length)
					} else {
						$.prompting('最多添加四个图片');
					}


				}
			});


			$(document).on('click', '.remove', function () {

				$(this).parents('li').remove()
			});


			//一键设置产品售价
			// $(document).on('click','.suremake',function(){
			$(document).on('click', '.suremake', function () {
				sells = parseInt($('.inputbox input').val());
				console.log(sells)
				for (i in message) {
					message[i].moneys = sells
				}
				if (isNaN(sells)) {
					return false
				}
				$('.bgcolor input').val(sells)
				for (var i = 1; i < $('tr').length; i++) {
					var sl = $('tr').eq(i).find('.table-left5').find('span').text()
					var lirun = $('tr').eq(i).find('.lirun').find('span').text(sells - sl)
					// console.log(lirun)
				}
				bstop = false;
				$(".cover").fadeOut(3000)
			})
			// $(document).on('change','.bgcolor input',function(){
			// 	var lr = $(this).val()
			// 	var lrs=$(this).parent().parent().siblings('.table-left5').find('span').text()
			// 	$(this).parent().parent().siblings('.lirun').find('span').text(lr-lrs)
			// })
			// })
			var sizeid = 1;
			var giftid = '';
			var num = '';
			var sz = '';
			var skuid = '';
			var dress = '';
			var kushi = '';
			var color = '';
			var moneys = '';
			var numbers = '';
			var img1 = '';
			var img2 = '';
			var shoumai = '';
			var sells = '';
			var bstop = true;
			var bq;
			var Attribute = [];
			var message = [];
			var gname = $('.namework').text();
			var Contents = $('.textwork').text();
			var a = '';
			var b = '';
			var remarks = '';

			//获取个人定制商品价格的接口
			//shopping(tid,sid,cid)
			function shopping(tid, sid, cid) {

				var dress = $('.left-top ul li.click2').text()
				var kushi = $('.left-style ul li.click').text()
				var color = $('.left-color ul li.clicks').attr('title')
				var colorid = $('.left-color ul li.clicks').attr('data-id')
				var size = $('.left-size ul li.click').text()
				var moneys = $('.left-size ul li.click').attr('data-moneys')
				var numbers = $('.left-size ul li.click').attr('data-numbers')
				var sizeid = $('.left-size ul li.click').attr('data-id')
				$('.yixuancont').text(dress + '/' + kushi + '/' + color)
				$('#chima ul > li').text(size)
				$('.money').find('i').text('¥' + moneys)
				$('.product-num').text(1)
				$('#kucun').text("(库存" + numbers + ")")
				shoumai +=
					`<tr>
				<td class="table-left table-left1">${dress}</td>
				<td class="table-left table-left2">${kushi}</td>
				<td class="table-left table-left3">${color}</td>
				<td class="table-left">${size}</td>
				<td class="table-left5">&yen;<span>${moneys}</span></td>
				<td>
					<div class="bgcolor">
						&yen;&nbsp;<input class="orange" readonly placeholder="0"></input>
					</div>
				</td>
				<td class="orange lirun">&yen;<span>0</span></td>
			</tr>`
				$('#trs').append(shoumai)
				message.push({
					colorid: colorid,
					sizeid: sizeid,
					numbers: 1,
					moneys: moneys
				})
				remarks = dress + '/' + kushi + '/' + color + '/' + size;
				/* $.ajax({
					type: "POST",
					url: 'WebJson.aspx?book=GetDzNumber',
					dataType: 'json',
					data: {
						tid: tid,
						sid: sid,
						cid: cid,
					},
					success: function (data) {
						console.log(data)
						dress = $('.left-top ul li.click2').text()
						kushi = $('.left-style ul li.click').text()
						color = $('.left-color ul li.clicks').attr('title')
						size = $('.left-size ul li.click').text()
						$('.yixuancont').text(dress + '/' + kushi + '/' + color)
						$('#chima ul > li').text(size)
						// var interText = doT.template($("#chima-template").text());
						// $("#chima").html(interText(data.date));
						for (var i = 0; i < data.date.length; i++) {
							shoumai +=
								`<tr>
    					<td class="table-left table-left1">${dress}</td>
    					<td class="table-left table-left2">${kushi}</td>
    					<td class="table-left table-left3">${color}</td>
    					<td class="table-left">${data.date[i].sizename}</td>
    					<td class="table-left5">&yen;<span>${data.date[i].moneys}</span></td>
    					<td>
    						<div class="bgcolor">
    							&yen;&nbsp;<input class="orange" readonly placeholder="0"></input>
    						</div>
    					</td>
    					<td class="orange lirun">&yen;<span>0</span></td>
    				</tr>`
							message.push({
								colorid: cid,
								sizeid: data.date[i].sizeid,
								numbers: 1,
								moneys: data.date[i].moneys
							})

						}

						$('#trs').append(shoumai)
						//尺码切换
						$('.chima ul li ').eq(0).addClass('click-size')
						sz = $('.chima ul li ').eq(0).text()
						console.log($('.chima ul li').eq(0).attr('data-money'))
						moneys = $('.chima ul li').eq(0).attr('data-money')
						numbers = $('.chima ul li').eq(0).attr('data-num')
						$('.money').find('i').text('¥' + moneys)
						$('.product-num').text(1)
						$('#kucun').text("(库存" + numbers + ")")
					}
				}) */
			}

			//remarks=dress+'/'+kushi+'/'+color+'/'+sz;
			/* $(document).on('click', '.chima ul li', function () {
				dress = $('.left-top ul li.click').text()
				kushi = $('.left-style ul li.click').text()
				color = $('.left-color ul li.clicks').find('div').text()
				$(this).addClass('click-size').siblings().removeClass('click-size')
				sizeid = $(this).attr('data-sizeid')
				sz = $(this).text()
				remarks = dress + '/' + kushi + '/' + color + '/' + sz;
			})
			$(document).on('click', '.chima ul li', function () {
				moneys = $(this).attr('data-money')
				numbers = $(this).attr('data-num')
				$('.money').find('i').text('¥' + moneys)
				//$('.product-num').text(numbers)
				num = numbers
			}) */
			num = $('.product-num').text()
			//个人定制题目和作品描述发生变化触发的事件
			// $('.namework').change(function(){
			// 	var namework=$(this).val()
			// 	$('.sheji').html(namework)
			// 	gname=namework
			// })
			//  $('.textwork').change(function(){
			// 	var textwork=$(this).val()
			// 	$('.miaoshu').html(textwork)
			// 	Contents=textwork
			// })

			//获取个人定制素材属性的接口
			$.ajax({
				type: "POST",
				url: 'WebJson.aspx?book=SelectPersonOrder',
				dataType: 'json',
				success: function (data) {
					console.log(data)
					// var interText = doT.template($("#mains-left-template").text());
					// $("#mains-left").html(interText(data[0].date));
					var interText = doT.template($("#sucai-template").text());
					$("#sucai").html(interText(data[0].date[4]));
					var sucaitext = '推荐';
					var sucaiid = $("#select-sucai").find("option:selected").val()
					// var sucaiid=$('#select-sucai').children('option').eq(0).val()
					//我的作品左边发生变化
					// 
					//我的作品右边发生变化$('.left-top ul li').eq(0).addClass('click')
					// $(document).on('click','.left-top ul li',function(){
					// 	$(this).addClass('click').siblings().removeClass('click')
					// })
					// $('.left-style ul li').eq(0).addClass('click')
					// $(document).on('click','.left-style ul li',function(){
					// 	$(this).addClass('click').siblings().removeClass('click')
					// })
					// $('.left-color ul li').eq(0).addClass('clicks')
					// $(document).on('click','.left-color ul li',function(){
					// 	var index=$(this).index();
					// 	var top =index*95+35+'px';
					// 	$(this).addClass('clicks').siblings().removeClass('clicks')
					// 	$(".color-span").css('top',top)
					// })
					$('.right-top>span').eq(0).addClass('click-right')
					$(document).on('click', '.right-top span', function () {
						var indexs = $(this).index()
						// $('.canvas-container').css('display','block')   
						$(this).addClass('click-right').siblings().removeClass('click-right')
						$('.right-content .content').eq(indexs).css('display', 'block')
						$('.right-content .content').eq(indexs).siblings().css('display', 'none')
					})
					$('.sucai-title span').eq(0).addClass('click-sucai')
					//素材的值发生变化的时候
					$(document).on('click', '.sucai-title span', function () {
						$(this).addClass('click-sucai').siblings().removeClass('click-sucai')
						sucaitext = $(this).text()
						var srcsucai = '';
						var sucaiimgs = '';
						$('#select-sucai').html('');
						$('.sucai-imgs').html('');
						//  $("#select-sucai").empty()
						// $(".sucai-imgs").empty()
						//素材库图片切换的数据
						$.ajax({
							type: "POST",
							url: 'WebJson.aspx?book=GetmdetailList',
							dataType: 'json',
							data: {
								id: '',
								code: sucaitext
							},
							success: function (data) {
								console.log(data)
								if (data.msg == "success") {
									for (var i = 0; i < data.typelist.length; i++) {
										srcsucai += '<option value="' + data.typelist[i].id + '">' + data.typelist[i].values + '</option>'
									}
									$('#select-sucai').html(srcsucai);
									for (var j = 0; j < data.date.length; j++) {
										sucaiimgs += `<li><img src="${data.date[j].imageurl}" class="img-polaroid"></li>`
										$('.sucai-imgs').html(sucaiimgs);
									}

								}

							}
						})
					})
					//素材的下拉列表发生变化的时候
					$(document).on('change', '#select-sucai', function () {
						sucaiid = $(this).val()
						// var srcsucai='';
						var sucaiimgs = '';
						$('.sucai-imgs').html('');
						// $("#select-sucai").empty()
						// $(".sucai-imgs").empty()
						//素材库图片切换的数据
						$.ajax({
							type: "POST",
							url: 'WebJson.aspx?book=GetmdetailList',
							dataType: 'json',
							data: {
								id: sucaiid,
								code: sucaitext
							},
							success: function (data) {
								console.log(data)
								if (data.msg == 'success') {
									// for (var i = 0; i < data.typelist.length; i++) {

									//            srcsucai +=`<option value="${data.typelist[i].id}">${data.typelist[i].values}</option>`
									//  }
									//     		$('#select-sucai').html(srcsucai);
									for (var j = 0; j < data.date.length; j++) {

										sucaiimgs += `<li><img src="${data.date[j].imageurl}" class="img-polaroid"></li>`
									}
									$('.sucai-imgs').html(sucaiimgs);
								}

							}
						})
					})
				}
			})
			//改变被选中的背景色
			// $("#post-way option:selected").css('background','#FF6700')
			// $("#post-way option").hover(function (){ 
			// 	alert() 
			//          // $(this).addClass('.change').siblings().removeClass("change")
			//      },function (){  
			//          // $(this).removeClass('change') 
			//      });
			//获取版权
			$.ajax({
				type: "POST",
				url: 'WebJson.aspx?book=GetDzService',
				dataType: 'json',
				success: function (data) {
					console.log(data)
					var interText = doT.template($("#banquan-template").text());
					$("#banquan").html(interText(data.date));
					bq = $("#banquan option:selected").val()
				}
			})
			$(document).on('change', '#banquan', function () {
				bq = $("#banquan option:selected").val()
				var bqtext = $("#banquan option:selected").text()
				$('#bqx').html(bqtext)
			})

			//当点击立即发布的时候生成商品 
			//   	gname=$('.sheji1').text()
			// Contents=$('.miaoshu1').text()
			$(document).on('click', '.fabu', function () {
				var tid = GetQueryString('tid')
				var sid = GetQueryString('sid')
				var gname = $('#namework').val();
				var Contents = $('#textwork').text();
				console.log(gname)
				if (bstop == false) {
					//bstop=true;
					//调用生成产品的接口
					if (inumber > 0) {
						uploadshopping1(gname, bq, Contents, tid, sid, tf, tb, message, Attribute)
					} else {
						$.MsgBox({
							type: "confirm",
							speed: 200,
							title: "",
							msg: '该产品未设计，确定发布吗？',
							opacity: '0.1',
							callback: function () {
								uploadshopping1(gname, bq, Contents, tid, sid, tf, tb, message, Attribute)
							}
						});
					}

				} else {
					$.prompting('请先设置产品售卖价格')
				}
			})

			function uploadshopping(gname, bq, Contents, typeid, styleid, a, b, message, Attribute) {
				$.ajax({
					type: "POST",
					url: 'WebJson.aspx?book=savepcgift',
					dataType: 'json',
					data: {
						gname: gname,
						bq: bq,
						Contents: Contents,
						tid: typeid,
						sid: styleid,
						imageurl1: a,
						imageurl2: b,
						message: JSON.stringify(message),
						Attribute: JSON.stringify(Attribute)
					},
					success: function (data) {
						console.log(data)


					}
				})
			}

			//当点击立即购买的时候，先生成产品 ，然后获取skuid，然后立即购买进入购买页面
			$(document).on('click', '.comebuy', function () {
				var tid = GetQueryString('tid')
				var sid = GetQueryString('sid')
				// if (bstop==false) {
				// 	bstop=true;
				//调用生成产品的接口
				gname = $('.namework').text();
				Contents = $('.textwork').text();
				if (gname == "") gname = '定制商品';
				if (Contents == "") Contents = '定制商品';
				if (inumber > 0) {

					console.log(gname)
					uploadshopping1(gname, bq, Contents, tid, sid, tf, tb, message, Attribute)
				} else {
					$.MsgBox({
						type: "confirm",
						speed: 200,
						title: "",
						msg: '该产品未设计，确定发布吗？',
						opacity: '0.1',
						callback: function () {
							uploadshopping1(gname, bq, Contents, tid, sid, tf, tb, message, Attribute)
						}
					});
				}

				// }else{
				// 	$.prompting('请先设置产品售卖价格')
				// } 
			})

			function uploadshopping1(gname, bq, Contents, typeid, styleid, a, b, message, Attribute) {
				$.ajax({
					type: "POST",
					url: 'WebJson.aspx?book=savepcgift',
					dataType: 'json',
					data: {
						uid: $.cookie('uid'),
						gname: gname,
						bq: bq,
						Contents: Contents,
						tid: typeid,
						sid: styleid,
						imageurl1: a,
						imageurl2: b,
						imageurl3: a,
						imageurl4: b,
						message: JSON.stringify(message),
						Attribute: JSON.stringify(Attribute)
					},
					success: function (data) {
						console.log(data)
						if (data.msg == 'success') {
							giftid = data.gid
							var cid = GetQueryString('cid')
							var tid = GetQueryString('tid')
							var sid = GetQueryString('sid')
							goods(cid, sid, tid, sizeid, giftid)
						} else {
							$.MsgBox({
								type: "alert",
								speed: 200,
								title: "",
								msg: data.describe,
								opacity: '0.1'
							});
						}

					}
				})
			}

			function goods(cid, sid, tid, sizeid, giftid) { //
				$.ajax({
					type: "POST",
					url: '/WebJson.aspx?book=CheckGift',
					dataType: 'json',
					data: {
						GiftId: giftid,
						ColorId: cid,
						SizeId: sizeid,
						StyleId: sid,
						TypeId: tid,
					},
					success: function (res) {
						console.log(res);
						if (res[0].msg == 'success') {
							skuid = res[0].date[0].id;
							buygoods(giftid, skuid, num, remarks)
						} else {
							$.MsgBox({
								type: "alert",
								speed: 200,
								title: "",
								msg: res[0].describe,
								opacity: '0.1'
							});

						}
					}
				})
			}

			function buygoods(giftid, skuid, num, remarks) {
				$.ajax({
					type: "POST",
					url: '/WebJson.aspx?book=BuyNow',
					dataType: 'json',
					data: {
						uid: $.cookie('uid'),
						GiftId: giftid,
						skuid: skuid,
						number: num,
						remarks: remarks
					},
					success: function (res) {
						console.log(res)
						if (res.msg == 'success') {
							window.location = 'submit-order.html';
							// $.MsgBox({type:"alert",speed:200,title:"",msg:data.describe,opacity:'0.1'});
						} else {
							if (res.describe == '会员ID丢失，请重新登陆以后再添加购物车!!') {
								$.MsgBox({
									type: "alert",
									speed: 200,
									title: "",
									msg: '请先登录或注册账号',
									opacity: '0.1',
									callback: function () {
										window.location = 'register-login.html';
									}
								});
							} else {
								$.MsgBox({
									type: "alert",
									speed: 200,
									title: "",
									msg: res.describe,
									opacity: '0.1'
								});
							}

						}
					}
				});
			}




			////fianlly 20180605
			getstyleData()

			function getstyleData() {

				var tid = GetQueryString('tid')
				var sid = GetQueryString('sid')
				if (!GetQueryString('tid')) tid = 1;
				if (!GetQueryString('sid')) sid = 1;
				$.ajax({
					type: "GET",
					url: '/WebJson.aspx?book=GetDzNew',
					dataType: 'json',
					data: {
						tid: tid,
						sid: sid
					},
					success: function (res) {
						if (res.msg == 'success') {
							var interTexta = doT.template($("#left-top-template").text());
							$("#left-top").html(interTexta(res.FuzhuangList));
							var interTextb = doT.template($("#left-style-template").text());
							$("#left-style").html(interTextb(res.clothingList));
							if (res.colorList.length > 0) {
								var sizedetail = res.colorList[0].sizedetail
								var interSize = doT.template($("#left-size-template").text());
								$("#left-size").html(interSize(sizedetail));
								$(".left-size ul li").eq(0).addClass('click')
							}
							var interTextC = doT.template($("#left-color-template").text());
							$("#left-color").html(interTextC(res.colorList));
							$('.filter-box').selectFilter({
								callBack: function (val) {
									console.log(val + '-是返回的值')
								}
							});

							$('.filter-title').val(GetQueryString('text'));
							$(".left-top ul li").each(function () {
								if ($(this).attr('data-id') == tid) {
									$(this).addClass('click2')
								}
							});

							$(".left-style ul li").each( function (index, val){
								if ($(this).attr('data-id') == sid) {
									$(this).addClass('click')
									// var sizeObject = res.clothingList[index]
									var sizeObject = {
										left1: 262,  // 正面 left
										top1: 131, // 正面top
										width1: 37, // 正面宽度
										height1: 41, // 正面长度
										left2: 129, // 背面left
										top2: 102, // 背面top
										width2: 146, // 背面宽度
										height2: 204, // 背面长度
									}
									window.localStorage.setItem('sizeObject', JSON.stringify(sizeObject))
								}
							});
							if (!GetQueryString('tid')) {
								$(".left-top ul li").eq(0).trigger("click");
							} else {
								$(".left-color ul li").eq(0).trigger("click");
							}


						}

					}
				});
			}
			$(document).on('click', '.left-top ul li', function () {
				$(this).addClass('click2').siblings().removeClass('click2')
				var tid = $(this).attr('data-id')
				var html = $(this).text()
				window.history.pushState({}, document.title, changeURLPar(document.URL, 'tid', tid));
				window.history.pushState({}, document.title, changeURLPar(document.URL, 'text', html));

				getstyleData()
				setTimeout(function () {
					$(".left-style ul li").eq(0).trigger("click");
					$(".left-size ul li").eq(0).trigger("click");
					$(".left-color ul li").eq(0).trigger("click");
				}, 100)




			})
			$(document).on('mouseover', '.left-top ul li', function () {
				$('.cimg').hide()
				$(this).find('.cimg').show()
				$(this).addClass('click2').siblings().removeClass('click2')


			})
			$(document).on('click', '.left-style ul li', function () {
				$(this).addClass('click').siblings().removeClass('click')
				var sid = $(this).attr('data-id')
				window.history.pushState({}, document.title, changeURLPar(document.URL, 'sid', sid));

				getstyleData()
				setTimeout(function () {
					$(".left-color ul li").eq(0).trigger("click");
				}, 100)


			})
			/* 点击选择尺寸 20181113 */
			$(document).on('click', '.left-size ul li', function () {
				$(this).addClass('click').siblings().removeClass('click')
				// var cid = $(this).attr('data-id')
				// window.history.pushState({}, document.title, changeURLPar(document.URL, 'cid', cid));
			})
			/* 点击选择尺寸 20181113 */
			//  此处为点击颜色
			$(document).on('click', '.left-color ul li', function () {
				var index = $(this).index();
				var top = index * 95 + 62 + 'px';
				$(this).addClass('clicks').siblings().removeClass('clicks')
				$(".color-span").css('top', top)
				// var cid = $(this).attr('data-id')
				// window.history.pushState({}, document.title, changeURLPar(document.URL, 'cid', cid));

				//shopping(tid,sid,cid)
				img1 = $(this).attr('data-img1')
				img2 = $(this).attr('data-img2')

				$('#tshirtFacing').attr('src', img1)
				$('#tshirtFacing').show();
				$('.zhengimg').attr('data-img1', img1)
				$('.fanimg').attr('data-img2', img2)
				$('#btn-center span').eq(1).trigger("click")
				$('#btn-center span').eq(0).trigger("click")
			})
			$('.backp').click(function () {

				$(".title-left").eq(0).trigger("click");

			})


			//20180903
			$(".img-title span").click(function () {
				$(this).addClass('click-sucai').siblings().removeClass('click-sucai')
				var index = $(this).index()
				if (index == 0) {
					$(".uplaodlayer").show()
					$(".toolslayer").hide()
				} else {
					$(".uplaodlayer").hide()
					$(".toolslayer").show()

				}


			});
		</script>

</body>

</html>
````
