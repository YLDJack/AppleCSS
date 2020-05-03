## 一、网站规划设计说明

1、结构设计

本网页以灰色为主色调，以表示缅怀的情感，渲染一种令人肃穆的气氛。页面的整体结构为上中下结构，网站的上端是黑色经典苹果导航条，是我根据苹果的官网仿照设计的。中间的部分防的是网页主体图片，下端为一些乔布斯的经典作品。底部为页脚。

2、内容规划

-  页面头部：设计网站LOGO标题：apple的logo，添加了搜索栏和各个网页的链接。

-  栏目导航：单击可以进入其它各内容页面，便于用户进入其他页面。

- 具体内容：本页的具体内容包括：缅怀乔布斯图片，以及乔布斯主要作品的图片，以及底部的一些列表。

-  版权声明：在页脚部分，另外有一些链接（本网页中没有实现链接）。


3、LOGO设计

本网页整体以灰色为主，蕴含一种缅怀之情，网页主体为一张乔布斯的图片，表明网页主要是为了纪念乔布斯，凸显本次设计网站的主题。

4、技术方案

（1）用photoshop软件对图片进行去水印处理，同时改变原有的图片的大小以适用于本网页。

（2）用Firewoorks软件用吸管工具对网站的背景颜色进行吸取，获得颜色的值，以便写入css代码；

（3）用Dreamweaver对网页进行代码的编写，以及用DIV+CSS进行优化处理；

（4）用photoshop对效果图进行切片处理，以及改变图片格式，获取一些网页的素材；

（5）用IE浏览器的F12开发者工具对apple的网页进行样式提取，以获取更好的界面效果。

## 二、网站色彩说明

1、网站主色调

该网站的主色彩是灰色和白色，配以少量的黑色，文字也为偏灰色，如下图所示：

![img](./images/applecss(1).jpg)

<center>图1 配色采集<center>

 

采用灰色的设计，是为了让其他颜色或装饰更加突出。灰色属于无彩色系。灰色给人感觉有点寂寞、捉摸不定，他代表乔布斯的去世这个世界的寂寞，灰色和白色的主题色调更加地凸显了我门的缅怀之情，使这个网站更契合主题。

2、网页链接色

表1 普通文字链接配色表

| 未访问过的链接(link) | 已访问过的链接(visited) | 鼠标悬停(hover) | 当前激活链接(active) |
| -------------------- | ----------------------- | --------------- | -------------------- |
| #666666,无下划线     | #666666,无下划线        | 无定义          | 无定义               |

 

3、 导航链接色

表2 导航链接配色表

| 未访问过的链接(link) | 已访问过的链接(visited) | 鼠标悬停(hover)   | 当前激活链接(active) |
| -------------------- | ----------------------- | ----------------- | -------------------- |
| #FFF,无下划线        | #FFF,无下划线           | #757575，无下划线 | 无定义               |

 

## 三、HTML页面结构图

![img](./images/applecss(2).jpg)

<center>图2 页面结构图</center>

 

## 四、页面DIV结构代码

```css
<div id="container">
  <div id=”menu”></div>
  <div id=”images”></div>
  <div id=”bottom”>
<div id=”bottom1”>
</div>
<div id=”bottom2”>
</div>
<div id=”bottom3”>
</div>
<div id=”bottom4”>
</div>
  </div>
  <div id=”footer”></div>
</div>
```



## 五、CSS代码及注释

```css
body{
	text-align:center;
	background-color:#F1F1F1;
	}
#container{
	width:1895px;
	margin:1px auto 0px auto;
	position:relative;
		
}
#menu {
		  font-family:Arial;
		  font-size:16px;
		  margin:0 0 0 0;
	  background: #323232;
		  padding-bottom:12px;
		  height:42px;
		  width:100%;
		  
}
#menu ul {
		  display:block;	
  		  padding:0 0 0 450px; 
   		  margin:0; 
          list-style-type:none;
          height:35px;
          }
#menu ul li {	  float:left;
		  }
#menu ul li a p{
		  display:block;
		  padding:0 87px 0 10px;
		  font-weight:400;
		  font-size:16px;
		  }
#menu #search{
	position:  absolute;
	top:15px;
	margin:0 0 0 5px;}
#menu #logo{
	padding:15px 87px 0 10px;
	}
#menu ul li a{
	text-decoration:none;
	color:#fff;
}
#menu ul li a:hover{
	color:#757575;}
#middle img{
	width:100%;
	height:795px;
}
#images{
	background-color:# FFF;}
#images ul li{
	list-style-type:none;
	top:850px;
	position: absolute;
	padding-top:5px;	
}
#images ul li.iPhone4s{	
	left:0px;}
#images ul li.iPad{
	left:475px;
}
#images ul li.iPod{
	left:955px;
}#images ul li.AppleStore{
	left:1420px;
}
#bottom{
	position:relative;
	top:190px;
	float:left;}

#bottom ul{
	list-style-type:none;
	font-size:1em;
	color:#666;
	font-size:12px;
	width:120px;
	text-align:left;
	}
#bottom  ul h3{
	font-size:12px;
	color:#333;
	width:100px;
	text-align:left;
	}
#bottom .bottom1{
	position: absolute;
	left:460px;}
#bottom .bottom2{
	position: absolute;
	left:655px;}
#bottom .bottom3{	position: absolute;
	left:850px;}
#bottom .bottom4{
	position: absolute;
	left:1048px;}
#bottom .bottom5{
	position: absolute;
	left:1240px;}
#footer{
	position: relative;
	top:410px;
	font-size:1em;
	clear:both;
	}
#footer ul {
	position: absolute;left:600px;
	list-style-type:none;
	
	}
#footer ul li {
	padding:0 10px 0 0;
	float:left;
	color:#666666;
	}
#footer ul li a{
	text-decoration:none;
	color:#666666;
	width:1px;
	}
</style>
```

## 六、页面测试结果

1、IE7.0下测试结果

![img](./images/applecss(3).jpg) 

![img](./images/applecss(4).jpg) 

2、FF下测试结果

![img](./images/applecss(5).jpg) 

![img](./images/applecss(6).jpg) 

## 七、心得体会。

 时间过得很快，一学期的web的学习要暂时告一段落了。作为一个这学期刚转专业到计科的学生，在刚开始接触各类专业课程的时候，都会有一些迷茫。但经过一段时间的学习，我感觉web是3门专业课程里最有意思的，也是最轻松的。这个学期，每节课都跟着刘老师打代码，逐渐的掌握ccs+div的应用。尤其是最后几节的综合应用，对作业中的排版和导航条设计帮助很大。

 这次大作业，主要是仿照苹果官网的界面设计，我很喜欢苹果的外观设计，同时作为一个果粉，也因此做了一个缅怀乔布斯的网页大作业。这次作业也花了很多时间用心去做，在搜寻素材的同时我发现了IE的F12的开发者工具。通过这个工具可以获取网的配色方案以及部分代码(PS:虽然以我现在的水平，大部分的代码还看不懂)，因此我可以很好的对我的网页进行排版很美化。至于底部的一些文字是为了不让网页看起太单调，从官网上摘取的，同时也能让网页更加美观。做css代码的时候也是按照要求一个一个盒子一层层的来设计，由于电脑本身的分辨率为1920x1080,所以整个网页的宽度将近为1920，没能设置1024的宽度(Ps:还望老师见谅)。

做网页的时候我感觉还是要一步一步来，和上面说的一样设计代码也要按顺序来和层次来一步步的设计（先大盒子再小盒子），同时做好位置和浮动。通过这次大作业的制作也让我巩固了本学期的web制作的知识。

以上就是我个人对于网页制作和这次大作业制作的一些心得，以后也希望能学习更多的网页设计的相关知识（JSP之类的），最后还是要谢谢刘老师这个学期的教学工作，对我的帮助很大。
