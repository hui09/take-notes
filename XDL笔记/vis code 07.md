## day7

visual studio code              : https://code.visualstudio.com/

阅读编译艺术：javascript:https://www.cnblogs.com/lhb25/p/javascript-book-2018.html

​                                                     https://www.runoob.com/html/html-tutorial.html



## DOM操作

	            DOM:使用javascript操作文档(元素)对象
	            BOM:使用javascript操作浏览器对象
	 1.操作有个元素的内容或者值
	            a.获取元素对象
	            var obj = docment.getElementById(id值);
	            ES6新标准
	                规定可以省略document.getElementById(),使用元素id,当做元素对象
	                <元素名称 id="d1"></元素名称>	
	                d1.innerHTML = "";		


​	
​	元素对象的值
​		a. 如果元素是 html对象
​			取值 var str = obj.innerHTML
​			赋值 obj.innerHTML = "值";
​		
​		b. 如果元素是 input 类型
​			取值 var str = obj.value
​			赋值 obj.value = "值";


	b.事件
	        onclick  单击事件
	        onmouseover 将鼠标移入到某元

