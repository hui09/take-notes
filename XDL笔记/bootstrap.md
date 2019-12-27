### day10

```
1.bootstrap 官方文档下载：https://v3.bootcss.com/
2.https://blog.csdn.net/ZT0518/article/details/82771429
		sodu  apt-get   install   smplayer  播放器下载  
3.npm下载     sodu    apt    install   npm
```

### 简介

```
bootstrap是由  Twitter公司的两名前端程序员研发的
是一套基于HTML 、CSS、JS 、技术的前段开源框架
bootstrap擅长响应式网页的开发  适用于移动端及PC端
```

### 使用步骤

```
 1.下载bootstrap框架文件
 2.解压得到三个文件夹将文件夹复制到项目的webcontent中
 				-  css   :    样式文件
 				-  fonts : 字体文件
 				-  js        :  脚本文件
 3.编写html
 4.引入Jquery；
 <script type="text/javascript"     src="js/jquery-3.2.1.min.js" ></script>
 5.引入Bootstrap.min.js   
 <script  type="text/javascript"    src="js/bootstrap.min.js"></script>
 6.引入bootstrap.css          
    <link  rel="stylesheet"       type="text/css"             href="css/bootstrap.css">
```

### 常用class                           

```
1.文本对齐方式
  class:
  		-  text-left         :   内容居中
  		-  text-center   :	 内容居中
  		- text-right       :    内容居右
```

### 列表的样式

```
class:
		- list-unstyled   :   取消前置的文字或图标，并取消左内边距
		- list-inline          :   取消前置的文字或图标，并取消左内边距  且所有li 设置为行内元素横向排列
		
```

###  代码块样式

```
原样显示代码块   ：		使用<pre>标签                   注：文本保留原来样式
bootstrap代码块 ：    div指定class="well",        注：文本显示一行
```

### 前景后景颜色

```
前景色(文本颜色)
                    class     :
                                    -		text-muted        : 	柔和灰	
                                    -		text-info   		   :	信息蓝
                                    -       text-primary	 :	  主要蓝
                                    -  		text-success	  :	   成功绿
                                    - 		text-warning 	:	 警告黄
                                    -       text-danger		  :	   危险红
```

```
后景色(背景颜色)
		有些特殊的后景色，因为颜色较深，bootstrap为了让文字能正常显示，文字颜色会被修改
                        class  :
                                    -	   bg-info				    :    	   信息蓝
                                    -	   bg-primary	      :		      主要蓝
                                    -	   bg-success		   :		   成功绿
                                    -	   bg-warning	      :		      警告黄
                                    -	   bg-danger	       :		    危险红
```

## 表格样式

#### 基本样式

```
class      :    table
```

#### 条纹表格样式

```
class      :	table   table-striped
```

#### 边框表格样式

```
class      :	table   table-bordered
```

#### 鼠标移入激活表格样式

```
class      : table table-hover
```

各种样式

```
class="table  table-hover     table-bordered   table-striped"                      
```

### 单独指定tr样式

```
给tr 添加class:
				-		active		       :		激活样式  半透明灰色
				-		success			 :		成功绿
				-		info				  :		信息蓝
				-		warning			:		警告黄
				-		danger			 : 		危险红
				- 		sr-only			   :		不显示
```

### 文字图标样式

```
使用步骤
			1.  编写span标签
			2. 设置span的class为文字图标class
						https://v3.bootcss.com/里面组件都是文字图标
						可以通过文字fongt-size:设置字体大小
			例如：
							class="span1            glyphicon  glyphicon-heart"
```

### 按钮样式：

```
按钮颜色样式
  				class    :
  								-			btn  btn-default    :   默认按钮
  								-			btn   btn-success  :   成功绿按钮
  								-			btn   btn-info			 :  信息蓝按钮
  								-			btn  btn-primary   :  主要蓝色按钮
  								-			btn  btn-warning   :   警告黄按钮
  								-			btn  btn-danger     :   危险红按钮
  								-            btn  btn-link			 :   超链接按钮
 可以将按钮的样式，添加到如下元素上：
                                1.   input  标签
                                2.   button 标签
                                3.   超链接a标签
      推荐               4.  span    标签      
     
     案例：
             <span      class="btn btn-default" >示例按钮input</span>
             <span     class="btn btn-success">示例按钮button</span>
            <span      class="btn btn-info">示例按钮a</span>
            <span      class="btn  btn-primary">示例按钮span</span>
            <span      class="btn  btn-warning">示例按钮span</span>
            <span      class="btn  btn-danger">示例按钮span</span>
            <span      class="btn  btn-link">示例按钮span</span>
```

### 按钮尺寸

```
class   :
			-			btn-lg  		 :		大按钮
			-			btn-sm		   :		小按钮
			-			btn-xs			 :		超小按钮
			-			btn-block	 :		块按钮，横向沾满一行，		
例如：
		    <span     class="btn btn-success  btn-lg">示例按钮button</span>
            <span      class="btn btn-success  btn-sm ">示例按钮a</span>
            <span      class="btn btn-success  btn-xs">示例按钮span</span>
            <span      class="btn btn-success btn-block">示例按钮span</span>	
```

#### 激活与禁用按钮

```
 	class：
 					-    active     :   激活
 					-   disabled   :  禁用   （仅仅是样式）
例如： 					
     <span     class="btn btn-success  active">激活样式</span>
     <span      class="btn btn-success   ">普通按钮</span>
     <span      class="btn btn-success disabled">禁用按钮</span>
```

### 移动设备优先（键值对）

```
手机屏幕，自适应大小
<meta name="viewport"   content="width=device-width,initial-scale=1,maximum-scale=1">
手机屏幕，自适应大小，禁用用户缩放
<meta name="viewport"   content="width=device-width,initial-scale=1,maximum-scale=1, user-scalable=no">
```

### 输入框样式

```
|   块输入框
		class   :   form-control
|   内联输入框
        1.当设备宽度小于768px时，自动切换为块输入框
        2.当我们设置了移动设备xiaoyu优先时，手机打开网页，缩小后的宽度常小于                            768px；
        3. 所有内联输入框，教响应式输入框，当手机打开时  横向撑开父元素，当电脑打开，就是普通的行内块元素，可以调整宽度
		
		
		1. 给form表单标签，添加class=form-inline
		2.给input 标签， 添加class=form-control
		
|	案例：
<div>
                <h3>用户注册</h3>
          <form  action=""   class="form-inline">
                  <p><input  placeholder="请输入账号"  class="form-control" ></input></p>
                   <p><input  placeholder="请输入密码"  class="form-control"></input></p>
                   <p><input  type="submit"  value="注册"  class="btn  btn-success   form- control" ></input></p>
            </form>
 </div>
```

### 输入框尺寸

```
|  class   :
			-    input-lg         :    大输入框
			-   input-sm        :  小输入框
|  案例：

<div>
      <h3>用户注册</h3>
       <form  action=""   class="form-inline">
           <p><input  placeholder="请输入账号"  class="form-control  input-lg"></p>   
           <p><input  placeholder="请输入密码"  class="form-control  input-lg"/></p>
           <p><input  type="submit"  value="注册"  class="btn  btn-success   form-control             btn-block  btn-lg" ></p>
         </form>		
```

### 响应式 

​                    4种   小于768   手机  ； 768-992 平板  ； 992-1200 电脑    ； 大于1200 电视

```
|  1.栅格系统 ：
			使用栅格系统，可以根据屏幕尺寸不同，来调整元素的宽度，
			栅格系统，将屏幕横向分为了12等份，元素的宽高，可以用栅格系统来指定占用的 份数。
|  2.栅格容器；
		两种容器（容器指的是被分为12份的元素）
		 a.固定宽度容器：     格式：<div  class="container"></div>;
		 
                               屏幕尺寸： a.手机屏幕(超小屏幕，小于768px);b.平板( 小屏幕768-992)
                                                  c.电脑屏幕( 中等屏幕 992-1200)   ；d.电视等大屏幕(大于1200)
                                容器宽度：a.100%      b.750px     c.970px      d.1170px
	     
	     b.撑满父元素的容器
					格式：		<div  class="container-fluid"></div>;							
```

### 栅格行：格式：<div  class="row"></div>

```
            栅格容器中的元素，必须编写在栅格行中
            栅格行横向能被占用12份， 当超出时，自动换行
```

### 栅格列的指定方式

```
a. 每种屏幕尺寸下，都用有12个不同的class，来描述元素占用的1份到12份。
b. 但是为了便于记忆，每种屏幕尺寸下的12class，前缀都是相同的，

c. 格式：
		屏幕尺寸：   a.手机屏幕(超小屏幕，小于768px);b.平板( 小屏幕768-992)
                                  c.电脑屏幕( 中等屏幕 992-1200)   ；d.电视等大屏幕(大于1200)  			
       
                  类  ：a. col-xs-数字        b. col-sm-数字        c.col-md-数字          d.col-lg-数字
                                                  
 注意：    四中屏幕规格，如果只是设置了较小的屏幕规格   ，较大的屏幕规格会自动按照较小的屏幕规格走，                                          
                                               
```



### 显示隐藏系统

```
       a.  屏幕尺寸： a.手机屏幕(超小屏幕，小于768px);b.平板( 小屏幕768-992)
                    c.电脑屏幕( 中等屏幕 992-1200)   ；d.电视等大屏幕(大于1200)  	
          b.  class值：
 超小屏幕显示,其他隐藏    :   visible-xs-参数         a.显示      b. 隐藏    c.隐藏     d.隐藏
 小屏幕显示,  其 他隐藏     :   visible-sm-参数        a.隐藏     b. 显示     c.  隐藏  d.隐藏
 中等屏幕显示, 其他隐藏   :   visible-md-参数      a.隐藏     b.隐藏      c.显示     d.隐藏
 大屏幕显示,  其他隐藏       :   visible-lg-参数         a.隐藏     b. 隐藏      c.隐藏     d.显示
      c.  参数：   值的是以什么样的元素分类显示，可选的值：  
                     inline/ inline-block /block
                      inline              :   将元素设置为行内元素，特点:不独占一行,
                     inline-block ：行内块，还是行内元素,也会具有块级元素的特点>可以设置宽度和高度
                      block              :   块级元素，独占一行
超小屏幕隐藏,其他显示  ：hidden-xs                    a.隐藏    b.显示    c.显示    d.显示
小屏幕隐藏,    其 他显示  ：hidden-sm                 a.显示    b. 隐藏   c.显示    d.显示
中等屏幕隐藏, 其他显示  ：hidden-md                a.显示    b. 显示   c.  隐藏  d.显示
大屏幕隐藏,     其他显示  ：hidden-lg                    a.显示    b.显示    c.  显示  d.隐藏
```

###  导航栏

```

a.步骤：
		1.编写ul标签，添加class属性  ；
        											|    class="nav  nav-tabs"( 横向导航栏)   
								                    | 	  class="nav "(纵向导航栏)
						     		                |     class="nav  nav-tabs    nav-justified"（横向撑满元素）
						     		                |     class="nav  nav-pills "(横向胶囊导航)
						     		                |      class="nav  nav-pills   nav-stacked"    (垂直胶囊导航)
						     		 
		2.添加子标签li,  li的包含一个个的超链接
b.案例：
		        <ul  class="nav  nav-tabs">
                                    <li><a href="#">首页</a></li>
                                    <li><a href="#">1</a></li>                 
                  </ul>
```

### 导航+内容切换

```
a.步骤：
		1.编写一个导航页
		2.在网页中编写一个div，用于显示内容，class="tab-content"
		3.给上述div，添加一个个的子div，每一个子div就是一个绑定导航项的内容
		4.给子div添加id，   并指定class="tab -pane  fade",  
		                                         默认显示的子div ，class="tab-pane  fade in  active"
		5.修改导航栏中的li标签里的a 标签，添加属性：data-toggle="tab"  href="#  子div的id"
		6.给默认的li，设置class="active"
b.案例：              
						<ul  class="nav  nav-tabs">
                                 <li    class="active"><a href="#div1"  data-toggle="tab">首页</a></li>
                                    <li><a href="#div2" data-toggle="tab">图片</a></li>
                                    <li><a href="#div3" data-toggle="tab">字符串</a></li>        
                       </ul>
                       <div class="tab-content">
                       < div  id="div1"      class="tab-pane  fade  in active">
                                          <h1>网站首页</h1>
                                           <p>这是及其正经的图</p>
                     </div>
                     <div  id="div2"   class="tab-pane  fade ">
                           <img  src=" image/qing.jpg"></img>
                    </div>
                     <div  id="div3"   class="tab-pane  fade  ">
                             <h3>snadufkhn</h3>
                    </div>
            </div>
```

### 下拉菜单

```
使用步骤：
		1.创建一个div（下拉菜单的容器），指定class="dropdown"或class="dropup"
		2.在上述创建的div 中添加的两个子元素
						第一个元素是点击的按钮，点击完毕弹出菜单，就是一个普通的按钮样式
						第二个子元素是弹出的菜单，是一个ul，包含一个个的li
		3.修改按钮
					-	给按钮添加属性：  data  toggle="dropdown"
					-	(可选的)给按钮添加一个向下的箭头，按钮添加span标签指定class="caret"					
	   4.修改ul(弹出的菜单)	
					-   ul标签添加class="dropdown menu"
					-  li中的每一个菜单项，都必须被超链接包含
	
	
案例：                   <span  class="caret"/>   箭头
                              <div  class="dropdown">
                                        <span  class="btn  btn-success"   data-toggle="dropdown">弹出菜单<span  class="caret">  </span >  </span>
                                          <ul  class="dropdown-menu">
                                                        <li><a href="#">笔记 </a></li>
                                                        <li><a href="#">书本 </a></li>
                                                        <li><a href="#">课程 </a></li>
                                                        <li><a href="#">本     </a></li>
                                                        <li><a href="#">地址 </a></li>
                                            </ul>
                                      </div>
```

### 下拉菜单的样式调整

```
-  设置菜单向上触发
          -   将外层div设置为  class="dropup"
-  设置菜单项在屏幕的右侧
         -   ul标签添加class="dropdown-menu-right"
-   设置弹出菜单的标题
		 -   给ul内部的前置一个新的li，li的内容是文本，  指定  li   的class="dropdown-header"
		
-   在多个菜单选项之间，添加分割线
	   	-   每一个分割线都是一个li  ，class="divider"
		
-    设置 某选项为禁用
		-   设置禁用选项  LI 的   class="disabled"
-    设置 菜单默认显示	
		-   在最外层的div中添加class="dropdown  open"
		
  案例：        
                              <div  class="dropdown"> 
                                <span  class="btn  btn-success"   data-toggle="dropdown">弹出菜单<span  class="caret"></span >                                    </span>
                                           <ul  class="dropdown-menu   dropdown-menu-right">
                                                   <li    class="dropdown-header"><a href="#">笔记 </a></li>
|设置分割线                              <li    class="divider"></li>
                                                   <li><a href="#">书本 </a></li>
|设置分割线                              <li    class="divider"></li>
                                                   <li><a href="#">课程 </a></li>
                                                  <li><a href="#">本     </a></li>
|设置分割线                          <li    class="divider"></li>
                                                   <li  class="disabled"><a href="#">地址 </a></li>
                                        </ul>
                            </div> 
```

<center ><h2>扩展</h2></center>
## 分裂式下拉菜单

----------------按钮组合  

```
步骤1：
		1.编写一个下拉菜单(按钮包含一个箭头)
		2.修改下拉菜单的  外层div 的class="btn-group"
		3.在最外层的div 中，前置一个按钮即可，
		
		
		
案例1：            <h2>按钮组合</h2>
             <div  class="btn-group"> 
                  <span  class="btn  btn-success">下载笔记</span>
                  <span  class="btn  btn-success"   data-toggle="dropdown"><span  class="caret"></span ></span>
                   <ul  class="dropdown-menu ">
                           <li  ><a href="#">下载课件</a></li>
                            <li><a href="#">下载书本 </a></li>
                            <li   ><a href="#">下载书</a></li>
                  </ul>
          </div> 
```

#### --分裂式下拉菜单

```
   
  步骤：
		1.编写一个下拉菜单(按钮包含一个箭头)
		2.修改下拉菜单的  外层div 的为class="input-group-btn"
		3.给当前编写的整个下拉菜单，添加父元素div，并指定class="input-group"
		4.给新加的父div，前置一个子元素，输入框，输入框的class的值：form-control
    
案例2：           
                   <div   class="input-group">
                             <input  type="text"  class="form-control">
                               <div  class="input-group-btn">
                                        <span  class="btn  btn-success"   data-toggle="dropdown">弹出菜单<span                                                class="caret">  </span >  </span>
                                                  <ul  class="dropdown-menu">
                                                        <li><a href="#">笔记 </a></li>
                                                        <li><a href="#">书本 </a></li>  
                                                 </ul>
                                      </div>
                             </div>
```

### 巨幕

```
与代码块的样式相似   ！在巨幕中出现的所有文本都会被放大  ！
实现步骤 ：给div添加class="jumbotron"
  案例：
  			<h1>巨幕中的h3标题</h1>
                  <div   class="jumbotron"  style="background-color:  aqua">
                            <h1>巨幕中的h3标题</h1>
                             <p>巨幕文本普通</p>
                 </div>
```

### 在导航中 加入下拉菜单

```
1.将导航的某一个选项，更改为下拉菜单的样式！
2.我们在编写导航时，是ul包含li
3.在编写下拉菜单时，最外层的父元素是div
4.li 与div 都是块元素   ！
5.在导航中加入下拉菜单的方式，就是将导航中的li  当作下拉菜单的div来编写，
	
	      总结：在导航中加入下拉菜单的方式，就是将导航中的一个li 当作下拉菜单的div来编写 ！
	      注意：下拉菜单中的按钮，不在使用span标签，而是使用超链接标签，并取消按钮样式 ！
	      
案例：
			 <ul  class="nav nav   nav-tabs ">
                          <li ><a href="javascript:void(0)">首页</a></li>
                         <li><a href="javascript:void(0)">图片</a></li>  
                         <li   class="dropdown">  
                                    <a  data-toggle="dropdown"   href="#">日韩 <span   class="caret"></span></a>
                                   <ul  class="dropdown-menu">
                                               <li>xiao</li>
                                                <li>2</li>
                                                 <li>3</li>
                                                  <li>4</li>
                                   </ul>
                        	 </li>
                 			 <li><a href="javascript:void(0)">你是</a></li> 
                 			  <li><a href="javascript:void(0)">你是</a></li> 
                 			   <li><a href="javascript:void(0)">你是</a></li> 
        </ul>
```



### 内容切换导航

```
步骤：
		1.  创建一个普通的导航
		2.  在导航ul的下面，添加一个兄弟元素div，指定div 的class="tab-content";
		3.   在上述创建的div中加入一个个的子div，每一个子div作为一个被切换的内容，
		        -|  这个div 必须有id，class值必须设置tab-pane  fade, 默认选中项的class值:tab-pane   fade  in  active
		 4.  导航中每一个超链接，添加属性：data-toggle="tab"
		 5.  导航中每一个超链接，都需要添加链接地址，链接地址为#第二步子div的id
		 6.   给导航中默认的li选项，设置class="active"，
		 
		 案例：
		 	  <ul class="nav  nav-tabs">
            <li class="active">
                  <a href="#t1" data-toggle="tab">首页</a>
            </li>
            <li>
                  <a href="#t2" data-toggle="tab">首页1</a>
            </li>
            <li>
                  <a href="#t3" data-toggle="tab">首页2</a>
            </li>
            <li>
                  <a href="#t4" data-toggle="tab">首页3</a>
            </li>
      </ul>
      <div class="tab-content">
            <div id="t1" class="tab-pane  fade   in  active">
                  <div class="jumbotron">
                        <h1>如果你觉得现在走的辛苦，那就证明你在走上坡路！</h1>
                        <p> 2.如果你足够努力，再加上一点点运气，你就会成功。 强者永远找方法！ 4.善用内在潜能，</p>
                  </div>
            </div>
            <div id="t2" class="tab-pane  fade">
                  <h3>日韩</h3>
                  <img src="image/t1.jpg"> </img> 
            </div>
                   <div id="t3" class="tab-pane  fade">
                        <h3>日本</h3>
                        <img src="image/t3.jpg" ></img> 
                  </div>
                         <div id="t4" class="tab-pane  fade">
                              <h3>更多内容</h3>
                              <img  src="image/qing.jpg" ></img>
                         </div> 
                        </div> 
```

### 附加导航

```
步骤：
		1.   通过栅格系统，实现左右两个div 的分割， 2:10
		           -左侧div  用于编写附加导航
		           -右侧div  用于编写内容
		2.   在左侧的div 中  加入普通的垂直导航
				    -给导航的 ul  标签，添加属性：data-spy="affix"
		3.    在右侧div ，与导航选项关联的位置，添加元素，并制定的id    ！
		4.    修改左侧 div 中的每一个导航的超链接，链接到指定的内容的#id
		5.    修改body  ，绑定导航到网页上，
		             - 给body 添加属性
		             						data-spy="scroll"  data-target="#左侧div的id"
		             						
		6.     给导航中默认的选项 li ，设置class="active"
		
		案例：
		<body  data-spy="scroll"  data-target="#menu">
                  <div  class="container">
                        <div  class="row">
                                <div  class="col-lg-2"   id="menu">
                                         <ul  class="nav nav-pills   nav-stacked"   data-spy="affix">
                                                                <li     class="active"><a href="#t1"  >第1章节 </a></li>
                                                                <li><a href="#t2">第2章节 </a></li>
                                                                <li><a href="#t3">第3章节 </a></li>
                                                    </ul>
                                </div>
                                <div  class="col-lg-10">
                                		<h3   id="t1">第1章节</h3>
                                		<p>...</p>
                                		<h3  id="t2">第2章节</h3>
                                		<p>...</p>
                                		<h3   id="t3">第3章节</h3>
                                		<p>...</p>
                                </div>
                        </div>
                  </div>
                </body>
```

### 导航条

```
一般用于网页顶部  与 底部的导航菜单   ！
使用步骤：
				1.  编写一个nav标签，指定class="navbar  navbar-default"
				2.  向nav标签中，加入ul标签，class="nav  navbar-nav"
				3.  向ul标签中 加入一个个的li   ，li的内容是超链接
				
	案例：
			<nav   class="navbar  navbar-default">
					<ul   class="nav navbar-nav">
								<li><a herf="#">首页</a></li>
								<li><a herf="#">首页1</a></li>
								<li><a herf="#">首页2</a></li>
								<li><a herf="#">首页3</a></li>
					</ul>
			<nav>
```

### 向导航中  加入其他的内容

```
1.   添加标题
           在nav标签中，前置一个div,     class="navbar-header"  ,div中包含一个span  ,span的class="navbar-brand"  ,  span的内容就是标题
         
          <div   class="navbar-header" >
                         <pan  class="navbar-brand"> java24.com <span>
            </div>
案例：
   				<nav   class="navbar  navbar-default">
   				         <div   class="navbar-header" >
                                       <pan  class="navbar-brand"> java24.com <span>
                         </div>
					<ul   class="nav navbar-nav">
								<li><a herf="#">首页</a></li>
								<li><a herf="#">首页1</a></li>
								<li><a herf="#">首页2</a></li>
								<li><a herf="#">首页3</a></li>
					</ul>
			<nav>
```

### 2.  添加表单

```
	步骤：  1.   给导航条中，正常加入一个from表单，指定from标签class="navbar-form"
						2.   可选操作：  建议将表单中的输入组件与提交按钮，设置为组合输入框  ！
						 <form  action="https://www.baidu.com/"   class="navbar-form"> </form>
						 			<div  class="input-group">
						 			          <input  type="text"   class="form-control"   name="wd"  placeholder="请输入搜索内容">
		                                       <span   class="input-group-addon"
				                               onclick="$(this).parent().parent().submit()">搜索</span>
						                    </div>
						      </from>
案例：
                    <nav   class="navbar  navbar-default">
                                    <div   class="navbar-header" >
                                               <span  class="navbar-brand"> java24.com <span>
                                    </div>
                                    <ul   class="nav navbar-nav">
                                                <li><a href="#">首页</a></li>
                                                <li><a href="#">首页1</a></li>
                                                <li><a href="#">首页2</a></li>
                                                <li><a href="#">首页3</a></li>
                                    </ul>
                    		 <form  action="https://www.baidu.com/s"   class="navbar-form"> 
						 			<div  class="input-group">
						 			          <input  type="text"   class="form-control"   name="wd"  placeholder="请输入搜索内容">
		                                       <span   class="input-group-addon"  onclick="$(this).parent().parent().submit()">搜索</span>
						             </div>
						      </form>
		  </nav>
```

### 3.控制导航中每个元素的显示位置

```
        	- 居左     ：  class="navbar-left"
			- 居右	  :    class="navbar-right"
```

 ### 4.可以通过给nav的所有子元素添加栅格系统的方式，来给导航条的内容，添加边距 ！

```
<nav>
		<div  class="container">....</div>
</nav>

案例：
            <nav   class="navbar  navbar-default">
      <div  style="width:1000px" margin:0px>  固定内容缩放不会改变样式，会自动加滚动条
            <div  class="container">
            		<div   class="navbar-header" >
            				<span  class="navbar-brand"> java24.com <span>
                    </div>
                            <ul   class="nav navbar-nav">
                            <li><a href="#">首页</a></li>
                            <li><a href="#">首页1</a></li>
                            <li><a href="#">首页2</a></li>
                            <li><a href="#">首页3</a></li>
                            </ul>
                    <form  action="https://www.baidu.com/s"   class="navbar-form"> 
                                <div  class="input-group">
                                         <input  type="text"   class="form-control   "   name="wd"   placeholder="请输入搜索内容">
                                         <span   style="top:0px" class="input-group-addon   glyphicon glyphicon-search"  onclick="$(this).parent().parent().submit()">搜索</span>
                                  </div>
                       </form>
                   </div>
             </nav>
```

### 5.  有时候需要在导航中  加入一些文字，发现这些文字与导航的部分 不对齐

```
|   给文字添加父元素span   指定span的class="navbar-text"
  指定固定宽度，浏览器窗口缩放元素不会变形换行 <div  style="width:1000px ; margin:  0  auto">  
```

### 6.固定导航条

```
           取消了导航条的圆角   ！
           根据设置的不同，漂浮在网页的顶部或底部
                    顶部：   添加nav标签的class="navbar-fixed-top"
                    低部：   添加nav标签的class="navbar-fixed-bottom"
```

### 7.静态导航条

```
			仅仅是取消了导航条的圆角
			        顶部：   添加nav标签的class="navbar-static-top"
```

### 分页标签

#### a.多页分页标签

```
步骤：
			1.   编写一个ul标签， 指定class="pagination"
			2.   给ul添加一个个li 标签,li 中的内牛容是一个个的超链接,每一个li 表示一个翻页的按钮
案例：
		<ul   class="pagination">
				<li><a href="#">首页</a></li>
				<li><a href="#">上一页</a></li>
				<li><a href="#">下一页</a></li>
		</ul>
```

#### b.上下翻页标签

```
步骤：
		1.  编写一个ul标签，指定class="pager"
		2.  给ul添加两个子标签li（li 中是超链接）
		               	-  第一个li   是上一页
		               	-  第二个li   是下一页
		3.   可选：
					    -   上一页居右    ： 给添加class="previous"
					    -   下一页居左    ：  给添加class="next"
案例：
		<ul   class="pagination">
				<li><a href="#">上一页</a></li>
				<li><a href="#">下一页</a></li>
		</ul>
```

### 警告框

```
在网页中添加警告框，显示时是占用网页空间的，可以被用户关闭的，关闭后不占用页面空间
		步骤：
        			1.编写一个div，   指定class="alert  alert-success"
        			2. 在div中，加入普通文字，表示弹出的文本内容  ！
        			3. 在div  中内容后置一个button标签 并设置class="close" 并添加属性data-dismiss="alert"  ,按钮需指定关闭的提示文字
        			
        			<div  class="alert  alert-success">
        			锄禾日当午，汗滴禾下土，谁知盘中餐.<button   class="close"  data-dismiss="alert">x</button>
        			</div>
```

### 栅格图片溢出处理

```
观察代码：
			<div  class="containner">
					<div  class="row">
							<div  class="col-lg-3"><div  class="thumbnail"><img    src="image/.jpg"></img></div></div>
							<div   class="col-lg-3"><div class="thumbnail" ><img    src="image/.jpg"></img></div></div>
							<div   class="col-lg-3"><div  class="thumbnail"><img    src="image/.jpg"></img></div></div>
					</div>
			</div>
           上述的代码，图片过大时，会溢出栅格显示，导致图片覆盖呈现。
如何解决：
		a.给栅格中的所有的img标签，添加父元素的div并指定div的   class="thumbnail"
				
案例：                
                <div  class="containner">
                  <div  class="row">
                              <div  class="col-lg-3"><div  class="thumbnail"><img    src="image/qing.jpg"></img></div></div>
                              <div   class="col-lg-3"><div class="thumbnail" ><img    src="image/t2.jpg"></img></div></div>
                              <div   class="col-lg-3"><div  class="thumbnail"><img    src="image/t3.jpg"></img></div></div>
                  </div>
      </div>
```

### 特殊的按钮

```
给普通的按钮样式，添加属性：data-toggle="button"

		案例：
				<span   class="btn  btn-success"   data-toggle="button">开关按钮</span>
```

### 单选按钮

```
步骤：
		1.   正常编写一组单选框（input标签  type="radio"）
		2.   给一组单选框中的  每一个input 标签添加父元素span ，并给span 指定任意按钮样式
		3.   通过给一组按钮样式的span添加父元素div ，来实现按钮组   ！
		    	-   div的  class="btn-group"
		    	-  属性：data-toggle="buttons"
案例：
		    	<div  class="btn-group"  data-toggle="buttons" >	
                        <span   class="btn btn-info"><input  type="radio"  name="sex"  value="1">男</span>
                        <span   class="btn btn-info"> <input  type="radio"  name="sex"  value="1">女</span>
                        <span   class="btn btn-info"><input  type="radio"  name="sex"  value="1">人妖</span>
                        <span   class="btn btn-info"><input  type="radio"  name="sex"  value="1">孙宽</span>
				</div>
```

### 复选按钮

```
使用步骤：
		与单选按钮一至，仅仅更改的是input标签的type="checkbox"
		
		<div  class="btn-group"  data-toggle="buttons" >	
                        <span   class="btn btn-info"><input  type="checkbox"  name="sex"  value="1">男</span>
                        <span   class="btn btn-info"> <input  type="checkbox"  name="sex"  value="1">女</span>
                        <span   class="btn btn-info"><input  type="checkbox"  name="sex"  value="1">人妖</span>
                        <span   class="btn btn-info"><input  type="checkbox"  name="sex"  value="1">孙宽</span>
				</div>
		
```

### 折叠面板

```
实现步骤：
		1.创建一个div   ，用作被折叠的内容div  ！ 指定class="coollapse",需要指定id 属性  
		2.在div前，创建一个按钮，用于点击展开面板
						属性：  data-toggle="collapse"   data-target="#内容div的id"
			
			
			<span  data-toggle="collapse"   data-target="#content"   class="btn btn-success">点击展开</span>
		<div  id="content"  class="collapse">
				<div  class="well">
                        <h3>折叠的内容</h3>
                         <p>一个人在其一生中</p>
                          <p>阅读一些立意深远</p>
                          <p>具有丰富哲学思考的散文</p>
		        </div>
		</div>
```

###  图片轮播组件

```
步骤：
		1.  编写一个div，是整个轮播图的容器， 
        		-  指定class="carousel  slide"
				-  属性data-toggle="carousel"
                -   给div添加id
                -   给div添加指定的宽度（宽度与图片素材等宽）
		
		2.  给上述的div，添加子元素div (包含图片内容的div)   指定class="carousel-inner"
	
       3.   在第二步创建的div中，加入一个个的子元素的div，每一个元素div  表示一个图片的容器
				-  class="item"
				- 默认显示的div  设置class="item  active"
				- 每一个div中，包含一个img标签
		
		4.  添加左右按钮 ，给第一步div添加  追加两个超链接子元素，并指定链接地址为第一步创建的div 的 #id
				- 第一个超连接 表示上一张    class="carousel-control    left"   data-slide="prev"  
				-  第二个超连接  表示下一张  class="carousel-control      right" data-slide="next"
		
		5.添加小圆点，给第一步添加的div ，追加一个ul标签，指定class="carousel-indicators"
				- 每一个li表示一个小圆点，数量与图片数量一致
				- 属性：  data-target="第一步创建的div的#id"   data-slide-to="对应图片的下标"
				- 默认选中的li   class="active"
		
		6.可选操作：
				-   自动轮播：  给第一步编写的div 添加属性：  data-ride="carousel"
				-   自动轮播间隔时长设置：  给第一步编写的div 添加属性： data-iterval="毫秒数"（默认值5000）
				
```

```
案例：
			<div  class="carousel  slide"  data-toggle="carousel"   id="xpage"   style="width:500px"   data-ride="carousel"    data-iterval="2000"   >
                                 <div  class="carousel-inner">
                                  <div  class="item  active"><img  src="image/1.jpg"></div>
                                  <div  class="item"><img  src="image/2.jpg"></img></div>
                                  <div  class="item"><img  src="image/3.jpg"></img></div>
                                   <div  class="item"><img  src="image/4.jpg"></img></div>
			           </div>
                                   <a  href="#xpage"   class="carousel-control       left"     data-slide="prev"  ></a>
                                    <a  href="#xpage"   class="carousel-control      right"  data-slide="next"></a>
			            <ul  class="carousel-indicators">
                                     <li  data-target="#xpage"   data-slide-to="0"   class="active">  </li>
                                     <li  data-target="#xpage"   data-slide-to="1">  </li>
                                     <li  data-target="#xpage"   data-slide-to="2">  </li>
                                      <li  data-target="#xpage"   data-slide-to="3">  </li>
			               </ul>
			</div>

```

### well

```

```



































