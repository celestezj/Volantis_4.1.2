---
layout: docs
sidebar: []
date: 2021-03-17 04:40:56
top_meta: false
bottom_meta: false
---

<!-- 卡通字体（CSS+JS）：要调节卡通字体的大小，设置dykatongcontent的font-size属性，要调节占地大小，调节dykatongwrapper的width（默认充满父容器100%）和height属性，且默认情况下dykatongwrapper是靠左的，可以通过margin来使其居（父容器之）中，你可以在任意页面使用该卡通字体，只要按照本示例规范地使用dykatongwrapper和dykatongcontent类并调用相应的渲染函数（一个页面只需要在底部调用一次）即可 -->
<div class="dykatongwrapper" style="text-align:center;width:60%;height:90px;margin:0 auto;">
  <div class="dykatongcontent" style="font-size:2.5rem">图像册</div>
</div>
<script>dykatongrender();</script>

<style type="text/css">
@import url("https://fonts.googleapis.com/css2?family=Indie+Flower&display=swap");
.flowerp{
	font-family: 'Indie Flower', cursive;
}
</style>
<p class="flowerp" style="text-align:center">暂时先随便找些图片占个位置~</p>

<!-- 图片翻转特效（纯CSS）：调节卡片大小很方便，除了修改dyalbumcard中的图片尺寸，还有字体大小以及line-height属性也要相应调整，具体见下面的span和p标签样式（原值分别为：320px，320px，span:20px&1px，p:16px&15px），由于此特效我只打算在相册页面使用，所以直接将全部CSS代码都放在此处了（注：本站所使用的特效全都来自“站长素材”） -->
<style type="text/css">
.dyalbumsection *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.dyalbumsection{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    transform-style: preserve-3d;
}
.dyalbumsection .dyalbumcard{
    position: relative;
    width: 180px;
    height: 180px;
    margin: 20px;
    transform-style: preserve-3d;
    perspective: 1000px;
}
.dyalbumsection .dyalbumcard .dyalbumbox{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    transform-style: preserve-3d;
    transition: 1s ease;
}
.dyalbumsection .dyalbumcard:hover .dyalbumbox{
    transform: rotateY(180deg);
}
.dyalbumsection .dyalbumcard .dyalbumbox .imgBx{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}
.dyalbumsection .dyalbumcard .dyalbumbox .imgBx img{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.dyalbumsection .dyalbumcard .dyalbumbox .contentBx{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #333;
    backface-visibility: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    transform-style: preserve-3d;
    transform: rotateY(180deg);
}
.dyalbumsection .dyalbumcard .dyalbumbox .contentBx div{
    transform-style: preserve-3d;
    padding: 20px;
    background: linear-gradient(45deg,#fe0061,#ffeb3b);
    transform: translateZ(100px);
}
.dyalbumsection .dyalbumcard .dyalbumbox .contentBx div span{
    color: #fff;
    font-size: 4px;
    letter-spacing: 1px;
}
.dyalbumsection .dyalbumcard .dyalbumbox .contentBx div p{
    color: #fff;
    font-size: 4px;
	line-height: 5px;
}
</style>

<section class="dyalbumsection">
	<div class="dyalbumcard">
		<div class="dyalbumbox">
			<div class="imgBx">
				<img src="https://cdn.jsdelivr.net/gh/celestezj/ImageHosting/img/20210318112621.png" alt="">
			</div>
			<div class="contentBx">
				<div>
					<span>Title</span>
					<p>Description</p>
				</div>
			</div>
		</div>
	</div>
	<div class="dyalbumcard">
		<div class="dyalbumbox">
			<div class="imgBx">
				<img src="https://cdn.jsdelivr.net/gh/celestezj/ImageHosting/img/20210318111545.jpg" alt="">
			</div>
			<div class="contentBx">
				<div>
					<span>Title</span>
					<p>Description</p>
				</div>
			</div>
		</div>
	</div>
	<div class="dyalbumcard">
		<div class="dyalbumbox">
			<div class="imgBx">
				<img src="https://cdn.jsdelivr.net/gh/celestezj/ImageHosting/img/20210318112617.jpg" alt="">
			</div>
			<div class="contentBx">
				<div>
					<span>Title</span>
					<p>Description</p>
				</div>
			</div>
		</div>
	</div>
	<div class="dyalbumcard">
		<div class="dyalbumbox">
			<div class="imgBx">
				<img src="https://cdn.jsdelivr.net/gh/celestezj/ImageHosting/img/20210318111432.jfif" alt="">
			</div>
			<div class="contentBx">
				<div>
					<span>Title</span>
					<p>Description</p>
				</div>
			</div>
		</div>
	</div>
	<div class="dyalbumcard">
		<div class="dyalbumbox">
			<div class="imgBx">
				<img src="https://cdn.jsdelivr.net/gh/celestezj/ImageHosting/img/20210318121345.gif" alt="">
			</div>
			<div class="contentBx">
				<div>
					<span>Title</span>
					<p>Description</p>
				</div>
			</div>
		</div>
	</div>
	<div class="dyalbumcard">
		<div class="dyalbumbox">
			<div class="imgBx">
				<img src="https://cdn.jsdelivr.net/gh/celestezj/ImageHosting/img/20210318111406.webp" alt="">
			</div>
			<div class="contentBx">
				<div>
					<span>Title</span>
					<p>Description</p>
				</div>
			</div>
		</div>
	</div>
</section>

<p class="flowerp" style="text-align:center">暂时先随便找些图片占个位置~</p>