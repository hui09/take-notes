### day 06

###  资料参考

```
1.流程图讲解：https://www.jianshu.com/p/b25085d309e5

2.流程图设计：https://www.jianshu.com/p/681273c790c2

3.思维导图教程：https://www.sohu.com/a/217127567_725657

4.在线流程图和思维导图工具：https://www.processon.com/
```

### c**语言内存与指针**

```
  linux  c语音编成基本原与实践   https://www.imooc.com/learn/248

​        liunx c语言指针和内存：       https://www.imooc.com/learn/394

​     *指针所指向的地址对应的值；

​         arr[5]: 表示跳过5个地址执行第五个

​ 1.  makeFile编译器：

​		   文件名：makefile:

	​		hello.out: max.o min.o hello.c
	
	​		                      gcc max.o  min.o hello.c -o  hello.out
	
	​		max.o:max.c
	
	​							  gcc   -c  max.c  
	
	​		min.o : min.c
	
	​							   gcc -c   min.c

     ​	      ./input.out                                   |                                    ./avg.out          						

​                 求和           输出             通过管道传输       输入        平均值
```

### C语言编程实践与原理

```

**C语言是一种通用的，过程式的编程语言，广泛用于系统与应用软件的开发**

**ANSI C ，由美国国家标准局为c语言制定的一套完整的国际标准语法**

* C语言的特点：

  简单，快速，高性能，兼容性好，功能强大，易于学习

  *  语言是基于UNIX开发的，所以使用c语言要在UNIX上。但windows是不兼容UNIX的，所以要下个虚 拟机来运行UNIX 
  *  下载Ubuntu镜像：www.ubuntu.org.cn 
  *  虚拟机：mac版：VMware Fusion 
  *  windows版：VMware Workstation 
  *  ubuntu 是个可以兼容linux的镜像系统

* #include  <stdio.h>(stdio.h 预装在Linux里面（标准输入输出库）)

* ```
  int main（）{}与void main（）{}区别
  int main要有返回值return，void main不用
  ```

  #include <stdio.h>

  int max(int a,int b)

  { 

   			if(a>b){

  ​					return a;

  ​					}else{

  ​					return b;

  ​				}

  }

  int main()

  {

  ​		int a1=33;

  ​        int a2=21;

  ​		int maxnum=max(a1,a2);

  ​		printf("the max value is %d\n", maxnum);

  ​		return 0;

  }

  * vim编辑的一些命令

    sp xx.xx 新建一个文件，分屏 

    shift +w + 切换 

  ​        set nu 调出行号 

  ​        -o 命名文件 

  ​        引入文件注意先声明 #include "xx.c"    

* makefile文件（用make命令执行）

  make:是一个非常重要的编译命令,本质上它是一个程序。利用make工具，可以将大型的开发项目分解成为多个更易于管理的模块，对于一个包括几百个源文件的应用程序，使用make和makefile工具就可以简洁明快地理顺各个源文件之间纷繁复杂的相互关系。
```

### 指针内存与变量

```
                *+任意参数或者变量均为指针参数或者变量  在调用该函数时需要在参数前+& 即：  change(&a,&b);

                变量前加*号表示加入指针。 在main函数中引用指针时是变量前加&号

                int *a=&b; a是指针，把b的地址赋给a，a指向b

                &取地址符

                指针变量不赋初值会出错，temp

                *指针变量 取指针所对应的值

                &整型变量 取整型所对应的地址

                一个字节八个二进制位

                计算机内存可以分为：系统内核，栈，堆，可自由分配，数据段，代码段

                编译之后的代码在代码段

                变量的本质就是一个地址标识符，指针保存的就是内存的地址

                栈保存的是函数当前执行的状态，栈的特点先进后出

                1、数组的指针 数组的指针其实就是数组在内存中的起始地址。而数组在内存中的起始地址就是数组变                     量名，也就是数组第一个元素在内存中的地址。 

                2、指向数组的指针变量 如果将数组的起始地址赋给某个指针变量，那么该指针变量就是指向数组的指                     针变量。
```



