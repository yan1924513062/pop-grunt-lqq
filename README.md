# 擦除组件效果说明 #
==============================================================
+ 1 组件介绍 面向对象实现弹窗，不需要依赖任何js库。
+ 2 在obj里边可以改参数，例如弹窗的宽高，背景颜色图片，字体边框阴影，标题，内容，字体大小等等
+ 3 步骤1：在html中添加一个按钮，例如：
+ <button type="button" class="btn btn-primary" data-toggle="popover" data-tip-class="popover-primary"data-placement="left">custom</button>
+ 步骤2：在src目录下main.js里边修改参数，例如：
+ var obj={
		id:"myPopover",						//div的id
		width:300,							//宽
		height:75,							//高
		fontsize:18,						//字体大小
		title:"江雪",						//标题
		content:"千山鸟飞绝，万径人踪灭。",	//内容
		border:"1px solid blue",			//边框颜色
		color:"red",						//字体颜色
		background:"#f1f1f1",				//背景颜色
		// backimg:"url('images/1.jpg') center center",//背景图片
		shadown:"10px 10px 5px 0px rgba(167,167,229, .7) inset",//边框阴影
		textShadow:"0px 0px 5px #f0f,0px 0px 10px rgba(1,0,1,0.8)",//字体阴影
	}
+ 步骤3：new一个 var pop1=new Pop(obj);