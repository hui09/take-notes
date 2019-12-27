## js训练

JS指南：https://www.cnblogs.com/lhb25/p/javascript-book-2018.html

JS参考手册:https://www.runoob.com/js/js-tutorial.html

## javaScript string

* indexOf()：

  检索字符串，indexOf() 方法可返回某个指定的字符串值在字符串中首次出现的位置。

  注意：对大小写敏感，如果要检索的字符串没有出现，则改方法返回-1。

* lastindexOf()：

  方法可返回一个指定的字符串值最后出现的位置，在一个字符串中的指定位置从后向前搜索

  注意：对大小写方法敏感

* slice(start,end):

  方法可提取字符串的某个部分，并以新的字符串返回被提取的部分。

  #### switch语句

  ```
  switch(表达式) {
       case n:
          代码块
          break;
       case n:
          代码块
          break;
       default:
          默认代码块
  } 
  ```

  switch语句每次只能计算一次switch表达式，把表达式的值与每个case值进行对比，

  如果存在匹配，则执行关联代码，

  default 关键词规定不存在 case 与表达式匹配时所运行的代码

* replace(n,m):

* 用于在字符串中用一些字符替换另一些字符，或替换一个与正则表达式匹配的子串

  n代表被替换的字符，m代表替换后的字符，m可以是函数而不是字符串。在这种情况下，每个匹配都调用该函数，它返回的字符串将作为替换文本使用。