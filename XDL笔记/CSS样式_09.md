# html 和CSS样式

css样式模板下载：http://www.csszengarden.com/tr/zh-cn/

css菜鸟教程：https://www.runoob.com/cssref/css3-pr-mediaquery.html

```
网站下载CHM：https://blog.csdn.net/Jason_fight/article/details/53339368
第一步  打开终端
第二步  更新代码库,指令为:sudo apt-get install update
第三步  安装软件,  指令为:sudo apt-get install kchmviewer
第四步  打开软件:在终端中输入 kchmviewer ,直接可以打开该软件
```



## 1.@media 查询

```
定义和使用： 
              a.使用 @media 查询，你可以针对不同的媒体类型定义不同的样式。
              b.@media 可以针对不同的屏幕尺寸设置不同的样式，特别是如果你需要设置设计响应式的页面，                                  @media是非常有用的。
              c.当你重置浏览器大小的过程中，页面也会根据浏览器的宽度和高度重新渲染页面。
              d.media   :  screen    常使用与电脑屏幕，平板电脑，智能手机            
实例：   <link   rel="stylesheet"     media="screen"    href="mystyle.css">       
```

###  2.pt 和 px 的区别：

```
  1.  pt 和 px 的转换规则其实很简单，转换公式为：pt=px 乘以 3/4。比如 1024px×3/4=768pt 大小。
  2. 使用 px 定义文字，无论用户怎么设置，都不会改变大小；使用 pt 定义文字，当用户设置超过 96DPI 的值，          数值越大，字体就越大。
```

### 3.[voice-family属性](https://www.cnblogs.com/nodot/articles/1872211.html)

```
#sidebar {
 padding: 10px;
 border: 5px solid black;
 width: 230px;    /*针对IE5*/
 voice-family: "\"}\"";
 voice-family: inherit;
 width: 200px;    /*实际的宽度*/
}  
这里使用voice-family属性，因为IE5无法读取voice-family属性，所以不会读取第二个width值
```

### 4. abbr(HTML)

```
注释某个单词：
                    <abbr  title="注释的etc缩写内容">etc</abbr>
                 鼠标放上后会显示title注释的内容，解释etc;
```

### 5.white-space属性指定元素内的空白怎样处理。

```
white-space :  段落中的文本不进行换行  
属性：
       normal           表示默认空白会被浏览器忽略。
		pre   :             空白会被浏览器保留。其行为方式类似 HTML 中的 <pre> 标签。
		pre-wrap     保留空白符序列，但是正常地进行换行。
		pre-line       合并空白符序列，但是保留换行符。
```

### 6.role ：(HTML)增强语义性

```
例如：role="article"   这是文章 帖子
             role 本质上是增强语义性，当现有的HTML标签不能充分表达语义性的时候，就可以借助role来说明。通常这种情况出现在一些自定义的组件上，这样可增强组件的可访问性、可用性和可交互性。
```

### 7. *font*

```
简写： font: 字体风格 || 字体变形 || 字体加粗 || 字体大小 || 字体的族科
```

```
例如：
.font{
font-style:italic;
font-variant:small-caps;
font-weight:bold;
font-size:12px;
line-height:1.5em;
font-family:arial,verdana;

font的简写注意事项
1、简写时，font-size和line-height只能通过斜杠 / 组成一个值，不能分开写。
      font{ font:italic  small-caps  bold   12px/1.5em    arial,verdana;}
```



