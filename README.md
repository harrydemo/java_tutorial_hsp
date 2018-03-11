# Youtube 视频:

+ [循序渐进学java从入门到精通 - 韩顺平](https://www.youtube.com/playlist?list=PL3rfV4zNE8CDPMYudVYZvNQU3LUQ72Mx0)

* <a href="http://www.youtube.com/watch?feature=player_embedded&v=gA-2WUsloqQ&list=PL3rfV4zNE8CDPMYudVYZvNQU3LUQ72Mx0" target="_blank">第00讲 开山篇</a>

# java平台

1. J2SE java开发平台标准版
2. J2EE java开发平台企业版


java程序需要在虚拟机上才可以运行，换言之只要有虚拟机的系统都可以运行java程序。不同系统上要安装对应的虚拟机才可以运行java程序

# 开发步骤

1. 编写源文件 (.java)
2. 编译源文件为类文件(.class)可用J2SE或J2EE编译
3. 在虚拟机上运行

# 注释

- //单行注释
- /* */多行注释

# java内容介绍

java编程可以分成三个方向：
1. java se (j2se)桌面开发  java中的基础中的基础
2. java ee (j2ee)web开发
3. java me (j2me)手机开发


# java se课程介绍
* <a href="http://www.youtube.com/watch?feature=player_embedded&v=bTThn0Dqe1k&list=PL3rfV4zNE8CDPMYudVYZvNQU3LUQ72Mx0&index=2" target="_blank">第01讲 内容介绍 项目演示 原理剖析</a>
- java面向对象编程(基础)
- java图开界面开发
- java数据库编程
- java文件io流编程
- java网络编程
- java多线程编程

# java ee基础1
- java面向对象编程--数据库编程-->java se
- java 基础2
- html--css--javascript-->div+css

# java ee中级部分
- Servlet--Jsp-->mvc模式

# java ee高级部分
- Struts--Ejb--Hibernate--Spring--Ajax(ext,dw2)-->ssh框架

## java之父gosling

[logo]: http://www.computinghistory.org.uk/userdata/images/medium/41/46/product-74146.jpg "James Gosling, the father of the Java programming language"

- 1990 sun启动 绿色计划
- 1992 创建oak语言-->java
- 1994 gosling参加硅谷大会演示java功能，震惊世界
- 1995 sun正式发布java第一个版本，目前最新是jdk7.0

# java开发工具
- 记事本、(jcreator、jbuilder退出舞台了)、netbean、eclipse
- 如何选择开发工具
- 先选择记事本，对java有一定了解后再使用eclipse高级开发工具
- 为什么呢？

1. 更深刻的理解java技术，培养代码感
2. 有利于公司面试

# java语言的特点
1. java语言是简单的
2. java语言是面向对象的
3. java语言是跨平台(操作系统)的[即一次编译，到处运行]
4. java是高性能的

# java第一个程序hello.java
运行java程序要安装和配置jdk
jdk是什么？
1. jdk全称java dvevlopment kit中文java开发工具包
2. jdk是sun公司开发的
3. jdk包括jre(java runtime envirnment)java运行环境、一堆java工具和java基础的类库(类共3600左右，常用类在150个左右)
4. 可以在www.sun.com下载
- 开发安装jdk,用户执行需要安装jre

# 配置JDK
- 添加环境变量即可
- windows下配置jdk
- 在计算机属性--高级设置--环境变量--添加PATH将JDK所在路径指定即可。多个环境变量设置时需要用;号进行隔开

1. 编写第一个hello.java
```java
//注释 (解释) 作者：
//功能：在控制台显示"hello"
//日期：2013.11.28
//public：表示这个类是公共的，一个java文件中只能有一个public类
//class：表示这是一个类
//hello：类名(公共类的类名必须和文件名一致)
public class hello{
      //一个主函数，相当于是程序的入口
      public static void main(String args[]){
        //执行语句
        //System：是一个包
        //out.println是输入函数
         System.out.println("hello!");
      }
}
```
2. 编译hello.java 使用javac hello.java
3. 执行hello.java 使用java hello

# java程序运行关系
1. java源文件(.java文件)
2. java编译器即javac.exe
3. java字节码文件(.class文件)
4. 由解释执行器即(java.exe)将字节码文件加载到java虚拟器(jvm)
5. 字节码文件(.class)就会在java虚拟机中执行

对hello.java程序进行改过使之变为一个简单的加法运算程序
```java
//注释 (解释) 作者：
//功能：在控制台显示"hello"
//日期：2013.11.28
//public：表示这个类是公共的，一个java文件中只能有一个public类
//class：表示这是一个类
//jiafa：类名(公共类的类名必须和文件名一致)
public class jiafa{
      //一个主函数，相当于是程序的入口
      public static void main(String args[]){
        //执行语句
        //System：是一个包
        //out.println是输入函数
        // System.out.println("hello!");
	    int a=10;//定义一个变量，变量名a，它的值10
	int b=20;//定义一个变量，变量名b，它的值20
        int result=a+b;//定义一个叫result变量将变量ab相加的值赋值给result
        //输出结果
        System.out.println("结果是"+result);
      }
}
```
----------------------------------------------------------------
为什么有变量
不论是使用哪种高级程序语言编写程序，变量都是其程序的基本组成单位。java中的基本数据类型的定义与c/c++中大体一致。
```java
public class Test{
	public static void main(String []args){
	  int a=1;//定义一个整形变量，取名a，并赋初值1
	  int b=3;//定义一个整形变量，取名b，并赋初值3
	  b=89;//给变量b赋89
	  System.out.println(a);//输出语句，把变量a的值输出
	  System.out.println(b);//把变量b的值输出
	}
}
```
----------------------------------------------------------------
# java基本语法---基本数据类型
java基本数据类型 四大类型
整数类型、小数(浮点)类型、布尔类型、字符类型

## 整数类型
可以表示一个整数，常用的整数类型有：byte,short,int,long

主要区别是 数据大小范围，请大家看一个小案例。
byte  占用内存 一个字节 范围：-128至127
short 占用内存 两个字节 范围：-32768至32767
int   占用内存 四个字节 范围：-2147483648至2147483647
long  占用内存 八个字节 范围：-?至?

## 小数(浮点)类型
可以表示一个小数，常用的小数(浮点)类型有：
float(单精度),double(双精度)
float 占用内存 四个字节 范围：3.4E-38至3.4E+38 只能提供7位有效数字
double占用内存 八个字节 范围：1.7E-308至1.7E+308 可提供16位有效数字

## 布尔类型
可以表示"真"或者"假"，类型是boolean
比如：
boolean spBool=true; //给变量spBool定义为boolean型并赋值为真

## 字符类型
可以表示 单个字符，字符类型是char。char是两个字节(可以存放汉字)
多个字符我们称为字符串，在java中String这种数据类型表示，但是String不是基本数据类型，而是类，类是复合数据类型。
结论：在java中，对char进行运算的时候，直接当做ascii码对应的整数对待。
思考：int test1='a'+'b';  输出值195
      char test2='a'+'b'; 输出值?
      char test3='中';    输出值195
 

# java基本语法--定义变量，初始化，赋值
## 定义变量
1、什么是定义变量？
int a; 这就是定义了一个变量，变量名是a
float haha;这也定义了一个变量，表示一个float类型的小数，变量名是haha

## 初始化变量
在定义变量的时候，就给值
int a=45;这就是初始化变量a
## 给变量赋值
比如你先定义了变量：int tt;
然后再给值tt=780;  ->这就是给变量赋值

----------------------------------------------------------------
# java基本语法--基本数据类型转换
## 自动转换
int a=1.2;     double b=3;
结论：数据类型可以自动的从低精度-->高精度。高精度不能转为低精度。
byte小于<short小于<int小于<long小于<float小于<double
在java中的小数默认是double数据类型
float赋值时要在值后加f
long赋值时要在值后加l

## 强制转换
如何把高精度转成低精度？
int a=(int)1.2;
练习int a=1;          int a=1;
    double b=4.5;     double b=4.5;
    a=b;              b=a;
    报错              成功

## 计算过程中的转换
int a=3;
int b=a+3.4;
结论：当一个整数和一个double运算的时候，运算结果会向高精度转换
 

# java 基本语法--运算符
java中常用的算术运算符是：+加、-减、*乘、/除、%取模
其实%运算可以得到两个数的余数。

## 算术运算符：++自加、--自减。
这两个运算符比较特殊，请大家思考一下：
int a=90;
a++;          等同于(a=a+1)
这时a等于？ 91

int b=89;
b--;          等同于(b=b-1)
这时b等于？ 88

int a=56;
int b=a++;  
System.out.println(b); 56
System.out.println(a); 57
***int b=++a;相当于a=a+1再将b=a；
   int b=a++;相当于b=a再将a=a+1。

----------------------------------------------------------------
## 算术运算符：+=左加、-=左减、/=左除、%=左取模
请大家看看几个案例，就明白了：
int a=90;
a+=90;           (相当于a=a+90)
请问，a现在等于多少？ 180

float b=89.7f;
b+=a;            (相当于b=b+a)
请问，b现在等于多少？ 269.7

int a=56;int b=90;
a-=34;b%=a;       (相当于a=a-34,b=b%a)
System.out.println(b); 2
System.out.println(a); 22
----------------------------------------------------------------

运算符
## 关系运算符
1、==等于；2、>大于；3、<小于；4、>=大于等于；5、<=小于等于；6、!=不等于
```java
	int a=90;int b=90;
	if(a==b){System.out.println("ok1");}
	b--;
	if(a>b){System.out.println("ok2");}
	if(a>=b){System.out.println("ok3");}
```
请编写一个程序，该程序可以接收两个数(可以是整数，也可是小数)并判断两个数是大于？小于？还是等于？
程序代码：
```java
import java.io.*;//载入IO流包
public class Demo5{
	public static void main(String []args){
	try{
	//输入流，从键盘接收数
	InputStreamReader isr=new InputStreamReader(System.in);
	BufferedReader br=new BufferedReader(isr);
	//给出提示
	System.out.println("请输入第一个数");
	//从控制台读取一行数据
	String a1=br.readLine();
	System.out.println("请输入第二个数");
	String a2=br.readLine();
	//把String转为float
	float num1=Float.parseFloat(a1);
	float num2=Float.parseFloat(a2);
	if(num1>num2){System.out.println("第一个大");}
	if(num1==num2){System.out.println("相等");}
	if(num1<num2){System.out.println("第二个大");}	
	}catch(Exception e){ 
	   e.printStackTrace();
	}
	}
}
```
----------------------------------------------------------------

## 运算符--逻辑运算符
用于判断逻辑关系的运算符
1、&&与；2、||或；3、!非
&&与的运算关系，真真为真，其它都为假。
||或的运算关系，假假为假，其它都为真。
!非的运算关系，真取假，假取真
请大家看个案例，请问输出什么：
```java
int a=90;int b=90;
if(a==b || a>8){System.out.println("ok1");}
b--;
if(a>b && a>45){System.out.println("ok2");}
if(!(a<=b)){System.out.println("ok3");}
```
# java基本语法----三大流程控制
## 顺序控制
听其名而知其意，让程序可以顺序的执行。
请大家看个案例[demo11.java]:
```java
int a=7;
System.out.println("a="+a);
System.out.println("hello!");
a++;
System.out.println("a="+a);
System.out.println("0(∩_∩)0");
a++;
System.out.println("a="+a);
```
## 分支控制
让程序有选择的执行，分支控制有三种：
1、	单分支；2、双分支；3、多分支a
1、单分支语法：
```java
	if(条件表达式){
		语句;
	}
```
2、双分支语法：
```java
	if(条件表达式){
		语句;
	}else{
		语句;
	}
```
3.1、多分支语法：
```java
	if(条件表达式){
		语句;
	}else if(条件表达式){
		语句;
	}else if(条件表达式){
		语句;
	}else{
		语句;
	}
```
3.2、多分支语法：
```java
	switch(条件表达式){ //***条件表达式数据类型，就和case常量表达式一致，否则就会报错。
	case 常量1:
		语句1;
			     //语句1至break中相当于{}可以加入相应程序代码
		break;  //break，表示跳出switch语句
	case 常量2:
		语句1;
		break;
		...
	case 常量n:
		语句n;
		break;
	default:
		语句;
		break;
	}
```
*****:switch中的可用数据类型主要是：允许byte,short,int,char,enum等

1、单分支控制作业：请大家看个案例[demo22.java]:
编写一个程序，可以输入人的年龄，如果该同学的年龄大于18岁，则输出“你年龄大于18，要为自己的行为负责!”

2、双分支控制作业：请大家看个案例[demo33.java]:
编写一个程序，可以输入人的年龄，如果该同志的年龄大于18岁，则输出“你年龄大于18岁，要对自己的行为负责!”否则，输出“你的年龄不大这次放过你了”

3、多分支控制作业：请大家看个案例[demo44.java]
编写一个程序，可以输入人的年龄，如果该同志的年龄大于18岁，则输出“你年龄大于18，要对自己的行业负责，送入监狱”。如果该同志的年龄大于10岁并且小于等于18，则输出“你的年龄也不小了，把你送少管所”。其它情况，则输出“小孩子，下次注意”。

4、多分支控制作业：请大家看个案例[demo55.java]
请编写一个程序，该程序可以接收一个字符，比如：a,b,c,d,e,f,g
a表示星期一，b表示星期二...根据用户的输入显示相应的信息，要求使用switch语句完成。

5、多分支控制作业：请大家看个案例[demo66.java]
对比switch与if语句在执行分支语句的区别。
***switch分支语句不支持判断类型即boolean类型，switch只支持byte,short,int,char,enum等数据类型
-------------------------------------------------------------------------------
 
## 循环控制
听其名而知其意，就是让你的代码可以循环的执行。
循环控制有三种
1、for循环 语法：
	for(循环初值;循环条件;步长){
		语句;  //循环体
	}

2、while循环 语法：
	while(循环条件){
		语句;  //循环体
	}
特别说明：while循环是先判断在执行语句。

3、do while循环 语法：
	do{
		语句;  //循环体
	}while(循环条件);
特别说明：do while循环是先执行，再判断。

请大家看个案例[demo77-88-99.java]:
编写一个程序，可以打印10句“你好，我是刘德华同志!”。请大家想想怎么做？
1、for循环
for (int a=0;a<10;a++){System.out.println("你好，我是刘德华同志!");}
2、while循环
int i=0;while(i<10){System.out.println("你好，我是刘德华同志!");i++;}
3、do while循环
int i=0;do{System.out.println("你好，我是刘德华同志!");i++;}while(i<10)

请编写一个程序，可以接收一个整数，表示层数，打印出金字塔一半。[demo100.java]
```java
***把一个复杂的问是先拆解成简单问题
//三角形[Demo100.java]
public class Demo100{
	public static void main(String []args){
		//死去活来法-->打四次
		int lay=4;
		//表示有多少层
		for(int i=1;i<=lay;i++){
			//打印*
			for(int j=1;j<=i;j++){
				System.out.print("*");
			}
			System.out.println();//换行
		}
	}
}
```
-------------------------------------------------------------------------------
```java
//金字塔[Demo101.java]
public class Demo101{
	public static void main(String []args){
		int lay=10;//表示有多少层
		for(int i=1;i<=lay;i++){
			//找出规律
			//1->3 2->2 3->1 4->0找出空格
			for(int k=1;k<=lay-i;k++){
			System.out.print(" ");
			}
			//打印*
			//1->1 2->3 3->5 4->7找出星的规律
			for(int j=1;j<=(i-1)*2+1;j++){
				System.out.print("*");
			}
			System.out.println();//换行
		}
	}
}
```
-------------------------------------------------------------------------------
```java
//镂空金字塔[Demo102.java]
public class Demo102{
	public static void main(String []args){
		int lay=10;//表示有多少层
		for(int i=1;i<=lay;i++){
			//找出规律
			//1->3 2->2 3->1 4->0找出空格
			for(int k=1;k<=lay-i;k++){
			System.out.print(" ");
			}
			//打印*
			//1->1 2->3 3->5 4->7找出星的规律
			for(int j=1;j<=(i-1)*2+1;j++){
				//判断该层是否是顶层或者是底层
				if(i==1||i==lay){
				System.out.print("*");
				}else{
					//如果是第一个*
					if(j==1||j==(i-1)*2+1){
					System.out.print("*");
					}else{
						System.out.print(" ");
					}
				}
			}
			System.out.println();//换行
		}
	}
}
```
-------------------------------------------------------------------------------
```java
//空心菱形[Demo103.java]
public class Demo103{
	public static void main(String []args){
		int lay=4;//菱形上半部行数
		for(int i=1;i<=lay-1;i++){ //判断循环上半部分
			for(int k=1;k<=lay-i;k++){ //找行内*号前输出空格
				System.out.print(" ");
			}
			for(int j=1;j<=(i-1)*2+1;j++){ //找行内输出星的位置
				if(j==1||j==(i-1)*2+1){  //判断行最小长度和最大长度，并在最小长度和最大长度上输出*号，行内输入出空格。
					System.out.print("*");
				}else{
					System.out.print(" ");
				 }
			}
			System.out.println(); //换行
		}
		for(int i=1;i<=lay;i++){  //判断循环菱形下半部分
			for(int k=1;k<=i-1;k++){ //判断循环找*号前要输出空格处
				System.out.print(" ");
			}
			for(int j=1;j<=(lay-i)*2+1;j++){ //判断循环行长度
				if(j==1||j==(lay-i)*2+1){ //判断行最小长度和最大长度，并在最小长度和最大长度上输出*号，行内输入出空格。
					System.out.print("*");
				}else{
					System.out.print(" ");
				 }
			}
			System.out.println();//输出换行
		}
	}
}
```
-------------------------------------------------------------------------------
```java
//实心菱形[Demo104.java]
public class Demo104{
	public static void main(String []args){
		int lay=4;//菱形上半部行数
		for(int i=1;i<=lay-1;i++){ //判断循环上半部分
			for(int k=1;k<=lay-i;k++){ //找行内*号前输出空格
				System.out.print(" ");
			}
			for(int j=1;j<=(i-1)*2+1;j++){ //找行内输出星的位置
				System.out.print("*");
			}
			System.out.println(); //换行
		}
		for(int i=1;i<=lay;i++){  //判断循环菱形下半部分
			for(int k=1;k<=i-1;k++){ //判断循环找*号前要输出空格处
				System.out.print(" ");
			}
			for(int j=1;j<=(lay-i)*2+1;j++){ //判断循环行长度
				System.out.print("*");
			}
			System.out.println();//输出换行
		}
	}
}
```
-------------------------------------------------------------------------------

# 1、java面向对象编程(1)-类与对象
一个问题？[Demo107.java]
张老太养了两只猫猫：一只名字叫小白，今年3岁，白色。还有一只叫小花，今年100岁，花色。请编写一个程序，当用户输入小猫的名字时，就显示该猫的名字，年龄，颜色。如果用户输入的小猫名错误，则显示张老太没有这只猫猫。
```java
//用前面学习过的知识写出代码
public class Demo107{
	public static void main(String []args){
		int a=49;//输入的名字49，50
		int cat1age=3; //第一只猫
		String cat1name="小白";
		String cat1color="白色";
		int cat2age=100; //第二只猫
		String cat2name="小花";
		String cat2color="花色";
		switch(a){
		case '1':
			System.out.println(cat1age+cat1color);
			break;
		case '2':
			System.out.println(cat2age+cat2color);
			break;
		default:
			System.out.println("张老太没有这只猫!");
		}
	}
}
```
## java语言是面向对象的
计算机语言的发展向接近人的思维方式演变
汇编语言 [面向机器]
c语言    [面向过程]
java语言 [面向对象]

# 类和对象的关系
把猫的特性提取出来-->猫类-->对象(实例)
                         -->对象(实例)
                         -->...
注意：从猫类到对象，目前有几种说法：1、创建一个对象；2、实例化一个对象；3、对类实例化...以后大家听到这些说法，不要模糊。(对象就是实例，实例就是对象)java最大的特点就是面向对象。
```java
//定义猫类
public class Demo105{
	public static void main(String []args){
		//创建一个猫对象
		Cat cat1=new Cat();//Cat是定义的一个数据类型
		//Cat cat1;
		//cat1=new Cat();// 等同于 Cat cat1=new Cat();
		//访问属性的 对象名.属性名字
		cat1.age=3;
		cat1.name="小白";
		cat1.color="白色";

		//创建第二只猫
		Cat cat2=new Cat();
		cat2.age=100;
		cat2.name="小花";
		cat2.color="花色";  
	}
}

//java中如何定义一个类？[类名的首写字母大写]可根据程序的需要定义类
class Cat{
	//下面的就是类的成员变量/属性
	int agr;
	String name;
	String color;
	Master myMaster;
}

//引用类型，比如建个主人类
class Master{
	int age;
	String name;
	String address;
}
```
类和对象的区别和联系
1、类是抽象的，概念的，代表一类事物，比如人类，猫类..
2、对象是具体的，实际的，代表一个具体事物
3、类对象的模板，对象是类的一个个体，实例

## 类--如何定义类
一个全面的类定义比较复杂，如：
package 包名;
class 类名 extends 父类 implements
接口名{
 成员变量;
 构造方法;
 成员方法;
}

要透彻的掌握类，必须要了解类的构成
class 类名{      ---->   待定...
  成员变量;
}

类--类的成员变量
成员变量是类的一个组成部分，一般是基本数据类型，也可是引用类型。比如我们前面定义猫类的int age 就是成员变量。

对象--如何创建对象
创建一个对象有两种方法
1、先声明再创建
 1、对象声明：类名 对象名
 2、对象创建：对象名=new 类名()

2、一步到位法
  类名 对象名=new 类名()

对象--如何访问(使用)对象的成员变量
  对象名.变量名; //简单先这样理解，以后加下控制符此表达就不准确了。
***对象总是存在内存中的

一个小思考题[Demo.105.java]
为了让大家加深印象，我们定义一个人类(Person)(包括名字、年龄)。用一步到位法去创建一个对象
	↓
我们看看下面一段代码:
```java
System.out.printlin(b.age);
Person a=new Person();         →           请问：b.age究竟是多少？
a.age=10;
a.name="小明";
Person b;
b=a;
```
***对象总是存在内存中的
一个小思考题[Demo106.java]
在明白对象是如何在内存中存在后，请大家再看看下面的思考题，请问会输出什么信息？
```java
Person1 a=new Person1();
a.age=10;
a.name="小明";
Person1 b;
b=a;
System.out.println(b.name);//输出“小明”
b.age=200;
System.out.println(a.age);//输出a.age为200
```
*****重点也是难点
类--成员方法的初步介绍
在某些情况下，我们要需要定义成员方法。比如人类：除了有一些属性外(成员变量表示的年龄、姓名...)，我们人类还有一些行为比如：可以说话、跑步..，通过学习，我们人类还可以做算术题。这时就要用成员方法才能完成。现在要求对Person类完善：
1、添加speak成员方法，输入出：我是一个好人
2、添加jisuan成员方法，可以计算从1+..+1000的结果
3、修改jisuan成员方法，该方法可以接收一个数n，计算从1+..+n的结果
4、添加add成员方法，可以计算两个数的和



# 类--类的成员方法(成员函数)定义
成员方法也叫成员函数，这里希望大家不要被两个名词搞晕了。
	public 返回数据类型 方法名(参数列表)
	{
		语句;//方法(函数)主体
	}
1、参数列表：表示成员函数输入
2、数据类型(返回类型)：表示成员函数输出
3、函数主体：表示为了实现某一功能代码块
```java
//类的调用及方法调用[Demo108.java]
public class Demo108{
	public static void main(String []args){
	Person p1=new Person();
	p1.speak();//调用speak方法
	p1.jiSuan();//调用计算方法
	p1.jiSuan(200);//调用可以传入参数的计算方法
	p1.add(12,10);//调用两个数的和
	
	int res=p1.add2(23,34);//调用两个数的和并返回值到res中
	System.out.println("res返回值是："+res);
	System.out.println("num1+num2+num3="+p1.add3(2,2.3f,4.5f));//返回类型一定要一致否则报错。
}
}
//定义名字的几个方法：
//1、驼峰法 如myCry；2、下划线法my_cry
//方法名在有不同参数的情况下可以使用同一个方法名，即有参数和没参数的方法可以同名
class Person{ //请注意类名首写字母应为大写如Person为类名 
	int age;
	String name;
	//1、可以输出我是好人方法
	public void speak(){  //请注意方法名的首写字母应为小写如speak为方法名
		System.out.println("我是一个好人");
	}
	//2、可以计算1+..+1000的方法
	public void jiSuan(){
		int result=0;
		for(int i=1;i<=1000;i++){
			result=result+i;
		}
	System.out.println("1+..+1000结果是"+result);
	}
	//3、带参数的成员方法,可以输入n值并计算1+..+n
	public void jiSuan(int n){
		int result=0;
		for(int i=1;i<=n;i++){
			result+=i;
		}
		System.out.println("1+..+n结果是"+result);
	}
	//4、计算两个数的和
	public void add(int num1,int num2){
		int result=0;	//与下面一句等同于return num1+num2;
		result=num1+num2;
		System.out.println("num1+num2="+result);
	}
	//5、计算两个数的和，并将结果返回给主调(调用它的)函数
	//注意：返回类型和返回结果的类型要一致
	//注意：在调用某个成员方法的时候，给出的具体数值的个数
	//和类型要相匹配。
	public int add2(int num1,int num2){
		return num1+num2;
	}
	//6、计算两个float数的和，并将结果返给主调函数
	public float add3(int num1,float num2,float num3){
		return num1+num2+num3;
	}
}
```
## 类--类的成员方法(函数)--如何理解
如何理解方法这个概念，给大家举个通俗的示例：
程序员调用方法：给方法必要的输入，方法返回结果。

类的成员方法--声明
public int test(int a);/*方法声明*/
这句话的作用是声明该方法，声明的格式为：
	访问修饰符 数据类型 函数名(参数列表);
在给Person类添加add方法的例题中，我们看到的关键字return，它的功能是把表达式的值返回的值返回给主调函数的方法。
	return 表达式;

类的成员方法(函数)--特别说明
1、方法的参数列表可以是多个
案例：在Person类中编写一个成员方法，从键盘输入三个数，返回最大的那个数。
参数列表可以是多个，并且数据类型可以是任意的类型int float double char..
	访问修饰符 返回数据类型 函数名(参数列表){
		语句; //函数主体
	}

2、方法可以没有返回值
案例：编写一个函数，从控制台输入一个整数打印出对应的金字塔。
返回类型可以是任意的数据类型(int,float,double,char..)也可以没有返回值void表示没有返回值
	访问修饰符 返回数据类型 函数名(形参列表){
		语句; //函数主体
	}

类的成员方法(函数)--小练习
案例：编写一个成员函数，从键盘输入一个整数(1-9)，打印出对应的乘法表[Demo110.java]
//实例键盘输入打印乘法表[Demo110.java]
```java
import java.io.*;
public class Demo110{
	public static void main(String []args){
		Cfb jiu=new Cfb();
			jiu.cf();
	}
}
class Cfb{
	public void cf(){
		try{
		//输入流，从键盘接收数
		InputStreamReader isr=new InputStreamReader(System.in);
		BufferedReader br=new BufferedReader(isr);
		//给出提示
		System.out.println("请输入1-9，按0退出:");
		//从控制台读取一行数据
		String a1=br.readLine();
		//把String转为int
		int num1=Integer.decode(a1);
			for(int i=1;i<=num1;i++){
				for(int j=1;j<=i;j++){
					System.out.print(i+"×"+j+"="+(i*j)+"\t");
				}
				System.out.println();			
			}
		}catch(Exception e){
		  e.printStackTrace();
		 }
	}
}
```
案例：编写函数，使给定的一个二维数组(3×3)转置

# 类定义的完善
在介绍了成员方法后，我们类的定义就可以完善一步：
class 类名{             class 类名{               待定
成员变量;     →        成员变量;           →         
}                       成员方法;
		                }

小结：1.先设计类；2.然后根据类创建对象。
小练习：
1、设计计算机类，要求如下：[Demo109.java]
属性：品牌(Brand)、颜色(Color)、cpu型号(CPU)、内存容量(Memory)、硬盘大小(Harddisk)、价格(Price)、工作状态(Work)
方法：打开(Open)、关闭(Close)、休眠(Sleep)
创建一个计算机对象，调用打开，关闭方法
```java
//计算机类与对象的代码
import java.io.*;//加载IO流包
public class Demo109{
	public static void main(String []args){
		Computer Pc=new Computer();
			Pc.Brand="品牌";
			Pc.Color="颜色";
			Pc.Cpu="Cpu型号";
			Pc.Memory="内存容量";
			Pc.Hd="硬盘容量";
			Pc.Price="价格";
			Pc.Work="工作状态";
			try{
			//输入流，从键盘接收数
			InputStreamReader isr=new InputStreamReader(System.in);
			BufferedReader br=new BufferedReader(isr);
			//给出提示
			System.out.println("请输入0-9控制机器");
			//从控制台读取一行数据
			String a1=br.readLine();
			//把String转为float
			float num1=Float.parseFloat(a1);
			if(num1==0){Pc.open();}
			else if(num1==1){Pc.close();}
			else if(num1==2){Pc.sleep();}
			else if(num1==3){System.out.println(Pc.Brand);}
			else if(num1==4){System.out.println(Pc.Color);}
			else if(num1==5){System.out.println(Pc.Cpu);}
			else if(num1==6){System.out.println(Pc.Memory);}
			else if(num1==7){System.out.println(Pc.Hd);}
			else if(num1==8){System.out.println(Pc.Price);}
			else if(num1==9){System.out.println(Pc.Work);}
			else {System.out.println("输入错误!");}	
			}catch(Exception e){ 
	   		e.printStackTrace();
			}
	}
}

class Computer{
	String Brand;
	String Color;
	String Cpu;
	String Memory;
	String Hd;
	String Price;
	String Work;
	public void open(){
		System.out.println("开机");
	}
	public void close(){
		System.out.println("关机");
	}
	public void sleep(){
		System.out.println("休眠");
	}
}
```
2、	采用面向对象思想设计超级马里奥游戏人物


-------------------------------------------------------------------------------

# 2、java面向对象编程(1)-构造方法(函数)
类的构造方法介绍
什么是构造方法呢？在回答这个问题之前，我们来看一个需求：前面我们在创建人类的对象时，是先把一个对象创建好后，再给他的年龄和姓名属性赋值，如果现在我要求，在创建人类的对象时，就直接指定这个对象的年龄和姓名，该怎么做？
			↓
你可以在定义类的时候，定义一个构造方法即可。

构造方法是类的一种特殊的方法，它的主要作用是完成对新对象的初始化。它有几个特点：
1、方法名和类名相同
2、没有返回值
3、在创建一个类的新对象时，系统会自动的调用该类的构造方法完成对新对象的初始化。
特别说明：
一个类可以定义多个不同的构造方法。
```java
//例人类构造方法[Demo111.java]
public class Demo111{
	public static void main(String []args){
		Person p1=new Person(12,"顺平");//给予不同的初始值，调用的构造方法不同，构造方法虽同名，但系统会根据初始值来选定构造方法。
	}
}
//定义一个人类
class Person{
	int age;
	String name;
	//默认构造方法
	public Person(){
	}
	//构造方法的主要用处是：初始化你的成员属性(变量)
	//构造方法
	public Person(int age,String name){
		System.out.println("我是构造1");
		age=age;
		name=name;
	}
	//构造方法2
	public Person(String name){
		System.out.println("我是构造2");
		name=name;
	}
}
```
类的默认构造方法
有些同志可能会问？亲爱的老师，我们在没有学习构造函数前不是也可以创建对象吗？
是这样的，如果程序员没有定义构造方法，系统会自动生成一个默认构造方法。比如Person类Person (){};
当创建一个Person对象时Person per1=new Person();默认的构造函数就会被自动调用。

类的构造方法小结：
1、构造方法名和类名相同；
2、构造方法没有返回值；
3、主要作用是完成对新对象的初始化；
4、在创建新对象时，系统自动的调用该类的构造方法；
5、一个类可以有多个构造方法；
6、每个类都有一个默认的构造方法。

类定义的改进
在提出构造方法后，我们类的定义就应该更加完善了：
class 类名{		class 类名{		class 类名{
成员变量;		成员变量;		成员变量;
}			→	成员方法;	→	构造方法;	→	待定..
				}				成员方法
								}
java面向对象编程(2)--this
一个问题？
请大家看一段代码：(Demo112.java)
*重点*：this是属于一个对象，不属于类的。
java虚拟机会给每个对象分配this,代表当前对象。坦白的讲，要明白this不是件容易的事
注意事项：this不能在类定义的外部使用，只能在类定义的方法中使用
```java
/*
	this的必要性
*/
public class Demo112{
	public static void main(String []args){
		Dog dog1=new Dog(2,"大黄");
		Person p1=new Person(dog1,23,"郭德纲");
		Person p2=new Person(dog1,24,"刘谦");
		p1.showInfo();	
		p1.dog.showInfo();
	}
}
//定义一个人类
class Person{
	//成员变量
	int age;
	String name;
	Dog dog;//引用类型
	public Person(Dog dog,int age,String name){
		//可读性不好
		//age=age;
		//name=name;
		this.age=age; //this.age指this代词指定是成员变量age
		this.name=name; //this.name指this代词指定是成员变量name
		this.dog=dog;
	}
	//显示人名字
	public void showInfo(){
		System.out.println("人名是："+this.name);
	}
}

class Dog{
	int age;
	String name;
	public Dog(int age,String name){
		this.age=age;
		this.name=name;
	}
	//显示狗名
	public void showInfo(){
		System.out.println("狗名叫"+this.name);
	}
}
```
-------------------------------------------------------------------------------
类变量--提出问题？
提出问题的主要目的就是让大家思考解决之道。
```java
public class Demo113{
	public static void main(String []args){
	/*	int total=0;
		Child ch1=new Child(3,"妞妞");
		ch1.joinGame();
		total++;
		Child ch2=new Child(4,"小小");
		ch2.joinGame();
		total++; 
	*/
		Child ch1=new Child(3,"妞妞");
		ch1.joinGame();
		Child ch2=new Child(4,"小小");
		ch2.joinGame();
		Child ch3=new Child(5,"大大");
		ch3.joinGame();
		System.out.println("共有="+Child.total);
	}
}
//定义小孩类
class Child{
	int age;
	String name;
	//static公共函数,total是静态变量，因此它可以被任何一个对象访问
	static int total=0; 
	public Child(int age,String name){
		this.age=age;
		this.name=name;
	}
	public void joinGame(){
		total++;
		System.out.println("有一个小孩加入了");
	}
}
```
-------------------------------------------------------------------------------
java面向对象编程(2)--类变量、类方法
什么是类变量？
类变量是该类的所有对象共享的变量，任何一个该类的对象去访问它时，取到的都是相同的值，同样任何一个该类的对象去修改它时，修改的也是同一个变量。

如何定义类变量？
定义语法：
	访问修饰符 static 数据类型 变量名;

如何访问类变量？
	类名.类变量名  或者  对象名.类变量名
```java
//类变量的程序演示[Demo114.java]
public class Demo114{
	static int i=1;
	static{
		//该静态区域块只被执行一次
		i++;
		System.out.println("执行一次");
	}
	public Demo114(){  //建立Demo114()构造函数
		System.out.println("执行二次");
		i++;
	}
	public static void main(String []args){
		Demo114 t1=new Demo114();  //创建t1对象实例并调用Demo114函数
		System.out.println(t1.i);

		Demo114 t2=new Demo114();
		System.out.println(t2.i);
	}
}
```
-------------------------------------------------------------------------------
什么是类方法，为什么有类方法？
类方法是属于所有对象实例的，其形式如下：
	访问修饰符 static 数据返回类型 方法名(){}
注意：类方法中不能访问非静态变量(类变量)。
使用：类名.类方法名 或者 对象名.类方法名
*重点*static静态的方法可以访问static静态变量，不能访问非静态变量(类变量)
      非静态方法可以访问非静态变量(类变量)同时也可以访问static静态变量。
```java
//统计总学费的程序代码，加深static静态的方法由静态变量的访问[Demo115.java]
public class Demo115{
	public static void main(String []args){
		//创建一个学生
		Stu stu1=new Stu(29,"aa",340);
		Stu stu2=new Stu(29,"aa",240);
		System.out.println(Stu.getTotalFee());
	}
}

//学生类
class Stu{
	int age;
	String name;
	int fee;
	static int totalFee;
	public Stu(int age,String name,int fee){
		this.age=age;
		this.name=name;
		totalFee+=fee;
	}
	//返回总学费[这是一个类方法(静态方法)]
	//java中规则：类变量原则上用类方法去访问或操作
	public static int getTotalFee(){
		return totalFee;
	}
}
```
类变量小结
1、什么时候需要用类变量
案例[Demo115.java]：定义学生类，统计学生共交多少钱？
用类变量，属于公共的属性
2、类变量与实例变量区别：
加上static称为类变量或静态变量，否则称为实例变量
类变量是与类相关的，公共的属性
实例变量属于每个对象个体的属性
类变量可以通过 [类名.类变量名]  直接访问
类方法小结
1、什么时候需要用类方法
案例[Demo115.java]：定义学生类，统计学生共交多少钱？
类方法属于与类相关的，公共的方法
实例方法属于每个对象个体的方法
类方法可以通过 [类名.类方法名]  直接访问

-------------------------------------------------------------------------------
# java面向对象编程的四大特征
抽象/封装/继承/多态

## 抽象
1、简单理解
我们在前面去定义一个类时候，实际上就是把一类事物的共有的属性和行为提取出来，形成一个物理模型(模版)。这种研究问题的方法称为抽象。

## 封装--什么是封装
封装就是把抽象出来的数据和对数据的操作封装在一起，数据被保护在内部，程序的其它部分只有通过被授权的操作(成员方法)，才能对数据进行操作。

封装--访问控制修饰符
电视机的开关，对音量，颜色，频道的控制是公开的，谁都可以操作，但是对机箱后盖，主机板的操作却不是公开的，一般是由专业维修人员来玩。那么java中如何实现这种类似的控制呢？不能随便查看人的年龄，工资等隐私[Demo116.java]
```java
//封装案例[Demo116.java]
public class Demo116{
	public static void main(String []args){
		//创建一个职员
		Clerk clerk1=new Clerk("小花",24,4567.6f);
		System.out.println("名字是"+clerk1.name+"薪水"+clerk1.getSal());
	}
}
//职员
class Clerk{
	public String name;
	//private私有的，public公有的
	private int age;
	private float salary;

	public Clerk(String name,int age,float sal){
		this.name=name;
		this.age=age;
		this.salary=sal;
	}
	//通过一个成员方法去控制和访问私有的属性
	public float getSal(){
		return this.salary;
	}
}
```
封装--访问控制修饰符
java提供四种访问控制修饰符号控制方法和变量的访问权限：
1、公开级别：用public修饰，对外公开
2、受保护级别：用protected修饰，对子类和同一个包中的类公开
3、默认级别：没有修饰符号，向同一个包的类公开
4、私有级别：用private修饰，只有类本身可以访问，不对外公开

4种访问级别的访问范围
|访问级别	|访问控制修饰符	|同类	|同包	|子类	|不同包|
--- | --- | ------ | --- | ------ | --- 
公  开	|Public	|√	|√	|√	|√
受保护	|Protected	|√	|√	|√	|╳
默  认	|没有修饰符	|√	|√	|╳	|╳
私  有	|private	|√	|╳	|╳	|╳

包--必要性
问题的提出，请看下面的一个场景[eclipse]
现在有两个程序员共同开发一个java项目，程序员xiaoming希望定义一个类取名Dog，程序员xiaoqiang也想定义一个类也叫Dog。两个程序员为此还吵了起来，怎么办？

包--三大作用
1、区分相同名字的类
2、当类很多时，可以很好的管理类
3、控制访问范围

包--换包命令
package com.自定义名字;
注意：打包命令一般放在文件开始处。

包--命名规范
小写字母  比如 com.sina.shunping

包--常用的包
一个包下，包含很多的类，java中常用的包有：
java.lang.* 包	自动引入	java.util.* 工具包
java.net.* 包	网络开发包	java.awt.* 包 窗口工具包

包--如何引入包
语法：import 包;
比如import java.awt.*;
我们引入一个包的主要目的要使用该包下的类

定义类的改进
在提出包后，我们类的定义就更加完善了：
class 类名{		class 类名{		class类名{		package包名;		待定..
成员变量;   →	成员变量;   →	成员变量;   →	class 类名{  →
}				成员方法;		构造方法;		成员变量;
				}				成员方法;		构造方法;
								}				成员方法;
												}
-------------------------------------------------------------------------------
## 继承--为什么有？[Demo117.java]
```java
//功能：说明继承的重要性

package com.abc;//包名
public class Demo117 {
	public static void main(String[] args) {
		Pupil p1=new Pupil();
		p1.printName();
	}
}

//将学生的共有属性提取，做一个父类
class Stu{
	//定义成员属性
	protected int age;
	public String name;
	public float fee;
	private String job;//私有将不被继承
	
	//编程中，如果你不希望子类继承某个属性或方法
	//则将其声明为private即可
	public void printName(){
		System.out.println("名字"+this.name);
	}
}

//小学生类
class Pupil extends Stu{
	//交学费
	public void pay(float fee){
		this.fee=fee;
	}
}
//幼儿
class Pre extends Pupil{
	//交学费
	public void pay(float fee){
		this.fee=fee*1.5f;
	}
}
//中学生类
class MiddleStu extends Stu{
	//交学费
	public void pay(float fee){
		this.fee=fee*0.8f;
	}
}
//大学生类
class ColStu extends Stu{
	//交学费
	public void pay(float fee){
		this.fee=fee*0.1f;
	}
}
```
继承--解决之道
继承可以解决代码复用，让我们的编程更加靠近人类思维。当多个类存在相同的属性(变量)和方法时，可以从这些类中抽象出父类(比如刚才的Student)，在父类中定义这些相同的属性和方法，所有的子类不需要重新定义这些属性和方法，只需要通过extends语句来声明继承父类：
	语法：class 子类 extends 父类
这样，子类就会自动拥有父类定义的某些属性和方法。

继承--深入讨论
1、父类的哪些属性(变量)、方法被子类继承了？并不是父类的所有属性、方法都可以被子类继承
	   父类						    子类
	public 属性;				public 属性;
	protected 属性;	    继承	protected 属性;
	private 属性;	     →				  属性;
			属性;
	public 方法;				public 方法;
	protected 方法;				protected 方法;
	private 方法;				          方法;
			方法;		
2、结论
从图可以看出，父类的public修饰符的属性和方法；protected修饰符的属性和方法；默认修饰符属性和方法被子类继承了，父类的private修饰符的属性和方法不能被子类继承。

继承--注意事项
1、子类最多只能继承一个父类(指直接继承)
2、java所有类都是Object类的子类 (所有的子类都可以逐级继承，例:爷->父->子->孙)
3、JDK6中有202个包3777个类、接口、异常、枚举、注释和错误
4、在做开发的时候，强烈建议大家多查jdk帮助文档
5、在使用类时，实在不知道怎么办，多使用搜索引擎

定义类的改进
在提出包后，我们类的定义就更加完善了：
class 类名{		class 类名{		class类名{		package包名;	
成员变量;   →	成员变量;   →	成员变量;   →	class 类名{  
}				成员方法;		构造方法;		成员变量;
				}				成员方法;		构造方法;
								}				成员方法;
												}   ↓
  ↓←←←←←←←←←←←←←←←←←←←←←←←←←
package 包名;
class 类名 extends 父类{		待定
	成员变量;			   →	....
	构造方法;
	成员方法;
}

-------------------------------------------------------------------------------
java面向对象编程(2)--方法重载(overload)
方法重载(overload)
按顺序，我们应该讲解多态，但是在讲解多态前，我们必须讲解方法重载和方法覆盖(override)。
请编写一个类(Abc)，编写方法可以接收两个整数，返回两个数中较大的数[Demo119.java]
//方法重载(overload)getMax
public class Demo119{
	public static void main(String []args){
		Abc2 abc1=new Abc2();
		System.out.println(abc1.getMax(12,14));
		System.out.println(abc1.getMax(24f,20f));
	}
}

class Abc2{
	//返回较大的整数
	public int getMax(int i,int j){
		if(i>j){
			return i;
		}else{
			return j;
		 }
	}
	public float getMax(float a,float b){
		if(a>b){
			return a;
		}else{
			return b;
		 }
	}
	//如果只是返回类型不一样，能否构成重载？不能够构成重载
/*	public double getMax(float d,double c){
		if(c>d){
			return c;
		}else{
			return d;
		 }
	}
	//如果只是控制访问修饰符不同，能否构成重载？不能够构成重载
	protected float getMax(float c,float d){
		if(c>d){
			return c;
		}else{
			return d;
		 }
	}*/
}

方法重载(overload)概念
简单的说：方法重载就是在类的同一种功能的多种实现方式，到底采用哪种方式，取决于调用者给出的参数。
注意事项：
1、方法名相同
2、方法的参数类型，个数，顺序至少有一项不同
3、方法返回类型可以不同(只是返回类型不一样，不能构成重载)
4、方法的修饰符可以不同(只是控制访问修饰符不同，不能构成重载)
 

方法覆盖(override)
既然子类可以继承父类的属性和方法，这样可以提高代码的复用性，这个很好，可是问题来了，假设现在我要求大家写三个类猫猫，狗狗，猪猪。我们知道这三个东东都是动物，动物必然存在相同的特点。根据类的抽象特征，我们可以把它们的相同点提取出来，形成一个父类，然后继承。
//子类方法覆盖父类方法[Demo120.java]
public class Demo120{
	public static void main(String []args){
		//创建一只猫
		Cat cat1=new Cat();
			cat1.cry();
		Dog dog1=new Dog();
			dog1.cry();
	}
}
//动物类
class Animal{
	int age;
	String name;
	//都会叫
	public void cry(){
		System.out.println("我是动物，不知道怎么叫");
	}

}
//猫猫类
class Cat extends Animal{
	//覆盖父类方法
	public void cry(){
		System.out.println("猫猫叫!");
	}
}
//狗狗类
class Dog extends Animal{
	//覆盖父类方法
	public void cry(){
		System.out.println("汪汪叫!");
	}
}

方法覆盖(override)概念
简单的说：方法覆盖就是子类有一个方法，和父类的某个方法的名称、返回类型、参数一样，那么我们就说子类的这个方法覆盖了父类的那个方法。比如上个案例的Cat类中的cry方法就覆盖了Animal类的cry方法。
注意事项：
方法覆盖有很多条件，有些书上说的比较细，总的讲有两点一定注意：
1、子类的方法的返回类型，参数，方法名称，要和父类的返回类型，参数，方法名称完全一样，否则编译出错。
2、子类方法不能缩小父类方法的访问权限。

===============================================================================
作业：上机实习题目
1、Josephu问题(丢手帕问题)
    Josephu问题为：设编号为1,2,...n的n个人围坐一圈，约定编号为k(1<=k<=n)的人从1开始报数，数到m的那个人出列，它的下一位又从1开始报数，数到m的那个人又出列，依次类推，直到所有人出列为止，由此产生一个出队编号的序列。
    提示：用一个不带头结点的循环链表来处理Josephu问题：先构成一个有n个结点的单循环链表，然后由k结点起从1开始计数，计到m时，对应结点的人从链表中删除，然后再从被删除结点的下一个结点又从1开始计数，直到最后一个结点从链表中删除算法结束。
//Josephu问题(丢手帕问题)
//使用单向链表
public class Demo121 {
	public static void main(String[] args) {
		CycLink cyclink=new CycLink();
		cyclink.setLen(5);//链表长度
		cyclink.createLink();
		cyclink.setK(2);//从第几个人开始数
		cyclink.setM(2);//数几下
		cyclink.show();
		cyclink.play();
	}
}

class Child{
	int no;
	Child nextChild=null;
	public Child(int no){
		//给一个编号
		this.no=no;
	}
}

//单向环形链表
class CycLink{
	//先定义一个指向链表第一个小孩的引用
	//指向第一个小孩的引用，不能动
	Child firstChild=null;
	Child temp=null;
	int len=0;//表示共有多少个小孩
	int k=0;
	int m=0;
	//设置m数几下
	public void setM(int m){
		this.m=m;
	}
	//设置环形链表大小
	public void setLen(int len){
		this.len=len;
	}
	//设置从第几个人开始数数
	public void setK(int k){
		this.k=k;
	}
	//开始play
	public void play(){
		Child temp=this.firstChild;
		//1.先找到开始数数的人
		for(int i=1;i<k;i++){
			temp=temp.nextChild;
		}
		while(this.len!=1){
			//2.数m下
			for(int j=1;j<m;j++){
				temp=temp.nextChild;
			}
			//找到要出圈的前一个小孩
			Child temp2=temp;
			while(temp2.nextChild!=temp){
				temp2=temp2.nextChild;
			}
			//3.将数到m的小孩，退出圈
			temp2.nextChild=temp.nextChild;
			//让temp指向下一个数数的小孩
			temp=temp.nextChild;
			this.len--;
		}
		//最后一个小孩
		System.out.println("最后出圈的小孩:"+temp.no);
	}
	
	//初始化单向环形链表
	public void createLink(){
		for(int i=1;i<=len;i++){
			if(i==1){
				//创建第一个小孩
				Child ch=new Child(i);
				this.firstChild=ch;
				this.temp=ch;
			}else{
				//创建最后一个小孩
				if(i==len){
					Child ch=new Child(i);
					temp.nextChild=ch;
					temp=ch;
					temp.nextChild=this.firstChild;
				}else{
					//继续创建小孩
					Child ch=new Child(i);
					temp.nextChild=ch;
					temp=ch;	
				}
			}
		}
	}
	//打印该环形链表
	public void show(){
		//定义一个跑龙套
		Child temp=this.firstChild;
		do{
			System.out.print(temp.no+" ");
			temp=temp.nextChild;
		}while(temp!=this.firstChild);
	}
}

 
java面向对象编程(2)--四大特征
多态--概念
所谓多态，就是指一个引用(类型)在不同情况下的多种状态。也可以理解成：多态是指通过指向父类的指针，来调用在不同子类中实现的方法。
实现多态有两种方式：1、继承；2、接口
多态演示[Dome122.java]
//演示继承、方法覆盖、多态
public class Demo122 {
	public static void main(String[] args) {
		//非多态演示
		Cat cat=new Cat();
		cat.cry();
		Dog dog=new Dog();
		dog.cry();
		//多态演示
		Animal an=new Cat();
		an.cry();
		an=new Dog();
		an.cry();
	}
}
//动物类
class Animal{
	String name;
	int age;
	public String getName() {
		return name;
	}
	public void setName(String name) {
		this.name = name;
	}
	public int getAge() {
		return age;
	}
	public void setAge(int age) {
		this.age = age;
	}
	//动物会叫
	public void cry(){
		System.out.println("不知道怎么叫");
	}
}
//创建Dog子类并继承Animal父类及覆盖cry方法
class Dog extends Animal{
	//狗叫
	public void cry(){
		System.out.println("汪汪叫");
	}
}
class Cat extends Animal{
	//猫自己叫
	public void cry(){
		System.out.println("猫猫叫");
	}
}
-------------------------------------------------------------------------------
多重多态演示[Dome123.java]
//演示子类继承父类、方法覆盖、多态方法
public class Demo123 {
	public static void main(String[] args) {
		//非多态演示
		System.out.println("非多态演示:");
		Cat cat=new Cat();
		cat.cry();
		Dog dog=new Dog();
		dog.cry();
		System.out.println();		
		//多态演示
		System.out.println("多态演示:");
		Animal an=new Cat();
		an.cry();
		an=new Dog();
		an.cry();
		System.out.println();	
		//多重多态演示
		System.out.println("多重多态演示:");
		Master master=new Master();
		master.feed(new Dog(),new Bone());
		master.feed(new Cat(),new Fish());
	}
}
//主人类
class Master{
	//给动物喂食物，使用多态，只要写一个方法
	public void feed(Animal an,Food f){
		an.eat();
		f.showName();
	}
}
//食物父类
class Food{
	String name;
	public void showName(){
		System.out.println("食物");
	}
}
//食物鱼子类
class Fish extends Food{
	public void showName(){
		System.out.println("鱼");
	}
}
//食物骨头子类
class Bone extends Food{
	public void showName(){
		System.out.println("骨头");
	}
}
//动物类Animal父类
class Animal{
	String name;
	int age;
	
	public String getName() {
		return name;
	}
	public void setName(String name) {
		this.name = name;
	}
	public int getAge() {
		return age;
	}
	public void setAge(int age) {
		this.age = age;
	}
	//动物会叫
	public void cry(){
		System.out.println("不知道怎么叫");
	}
	//动物吃东西
	public void eat(){
		System.out.println("不知道吃什么");
	}
}
//创建Dog子类并extends继承Animal父类及覆盖cry方法
class Dog extends Animal{
	//狗叫
	public void cry(){
		System.out.println("汪汪叫");
	}
	//狗吃东西
	public void eat(){
		System.out.println("狗爱吃骨头");
	}
}
class Cat extends Animal{
	//猫自己叫
	public void cry(){
		System.out.println("猫猫叫");
	}
	//猫吃东西
	public void eat(){
		System.out.println("猫爱吃鱼");
	}
}

多态--注意事项：
1、java允许父类的引用变量引用它的子类的实例(对象)
Animal an=new Cat();//这种转换时自动完成的
2、关于类型转换还有一些具体的细节要求，我们在后面还要提，比如子类能不能转换成父类，有什么要求等等...

-------------------------------------------------------------------------------
java面向对象编程(3)--抽象类
抽象类--解决之道
当父类的一些方法不能确定时，可以用abstract关键字来修饰该方法[抽象方法]，用abstract来修饰该类[抽象类]。
//抽象类的必要性[Demo124.java]
public class Demo124 {
	public static void main(String[] args) {
		//Animal an=new Animal();抽象类不允许实例化
		Animal an=new Cat();
		an.cry();
		an=new Dog();
		an.cry();
	}
}
//抽象类abstract关键词
abstract class Animal{
	String name;
	int age;
	//动物会叫，使用了abstract抽象方法
	abstract public void cry();//抽象类中可以没有abstract抽象方法
	//抽象类内可以有实现方法
	public void sx(){
		System.out.println("实现方法");
	}
}
//当一个子类继承的父类是abstract抽象类的话，需要程序员把抽象类的抽象方法全部实现。
class Cat extends Animal{
	//实现父类的cry，其实类似上节学习中的子类覆盖父类
	public void cry(){
		System.out.println("猫猫叫");
	}
}
class Dog extends Animal{
	//实现父类的cry，其实类似上节学习中的子类覆盖父类
	public void cry(){
		System.out.println("汪汪叫");
	}
}

抽象类--深入讨论
抽象类是java中一个比较重要的类。
1、用abstract关键字来修饰一个类时，这个类就是抽象类。
2、用abstract关键字来修饰一个方法时，这个方法就是抽象方法。
3、abstract抽象类中的abstract抽象方法是不允许在抽象类中实现的，一旦实现就不是抽象方法和抽象类了。abstract抽象方法只能在子类中实现。
4、抽象类中可以拥有实现方法。
5、抽象方法在编程中用的不是很多，但是在公司笔试时，却是考官比较爱问的知识点。

抽象类--注意事项
1、抽象类不能被实例化
2、抽象类不一定要包含abstract方法。也就是说，抽象类可以没有abstract抽象方法。
3、一旦类包含了abstract抽象方法，则这个类必须声明为abstract抽象类。
4、抽象方法不能有主体。
	正确的抽象方法例：abstract void abc();
	错语的抽象方法例：abstract void abc(){} 

java面向对象编程(3)--接口
接口--为什么有？
USB插槽就是现实中的接口。
什么是接口？
接口就是给出一些没有内容的方法，封装到一起，到某个类要使用的时候，在根据具体情况把这些方法写出来。
接口的建立语法：interface 接口名{方法;}
语法：class 类名 implements 接口{
		方法;
		变量;
	}
小结：接口是更加抽象的抽象的类，抽象类里的方法可以有方法体，接口里的所有方法都没有方法体。接口体现了程序设计的多态和高内聚低偶合的设计思想。

接口--注意事项
1、接口不能被实例化
2、接口中所有的方法都不能有主体。错误语法例：void aaa(){}←(注意不能有花括号)
   接口可以看作更加抽象的抽象类。
3、一个类可以实现多个接口
4、接口中可以有变量[但变量不能用private和protected修饰]
  a、接口中的变量，本质上都是static的而且是final类型的，不管你加不加static修饰
  b、在java开发中，我们经常把常用的变量，定义在接口中，作为全局变量使用
		访问形式：接口名.变量名
5、一个接口不能继承其它的类，但是可以继承别的接口

//接口的实现[Demo125.java]
//电脑，相机，u盘，手机

//usb接口
interface Usb{
	int a=1;//加不加static都是静态的，不能用private和protected修饰
	//声明了两个方法
	public void start();//接口开始工作
	public void stop();//接口停止工作
}
//编写了一个相机类，并实现了usb接口
//一个重要的原则：当一个类实现了一个接口，要求该类把这个接口的所有方法全部实现
class Camera implements Usb{
	public void start(){
		System.out.println("我是相机，开始工作了..");
	}
	public void stop(){
		System.out.println("我是相机，停止工作了..");
	}
}
//接口继承别的接口
class Base{
}
interface Tt{
}
interface Son extends Tt{
}
//编写了一个手机，并实现了usb接口
class Phone implements Usb{
	public void start(){
		System.out.println("我是手机，开始工作了..");
	}
	public void stop(){
		System.out.println("我是手机，停止工作了..");
	}
}
//计算机
class Computer{
	//开始使用usb接口
	public void useUsb(Usb usb){
		usb.start();
		usb.stop();
	}
}
public class Demo125 {
	public static void main(String[] args) {
		System.out.println(Usb.a);
		//创建 Computer
		Computer computer=new Computer();
		//创建Camera
		Camera camera1=new Camera();
		//创建Phone
		Phone phone1=new Phone();
		computer.useUsb(camera1);
		computer.useUsb(phone1);
	}
}
-------------------------------------------------------------------------------
 

定义类的改进
有了接口，我们类的定义就更加完善了：
class 类名{		class 类名{		class类名{		package包名;	
成员变量;   →	成员变量;   →	成员变量;   →	class 类名{  
}				成员方法;		构造方法;		成员变量;
				}				成员方法;		构造方法;
								}				成员方法;
												}   ↓
  ↓←←←←←←←←←←←←←←←←←←←←←←←←←
package 包名;				package 包名;
class 类名 extends 父类{	class 类名 extends 父类 implements 接口名{
	成员变量;	  		 →		成员变量;
	构造方法;					构造方法;
	成员方法;					成员方法;
}							}
-------------------------------------------------------------------------------
实现接口VS继承类
java的继承是单继承，也就是一个类最多只能有一个父类，这种单继承的机制可保证类的纯洁性，比C++中的多继承机制简洁。但是不可否认，对子类功能的扩展有一定影响。所以：
1、实现接口可以看作是对继承的一种补充。(继承是层级式的，不太灵活。修改某个类就会打破继承的平衡，而接口就没有这样的麻烦，因为它只针对实现接口的类才起作用)
2、实现接口可在不打破继承关系的前提下，对某个类功能扩展，非常灵活。

//实例：建立子类并继承了父类且连接多个接口[Demo126.java]
public class Demo126 {
	public static void main(String[] args) {
		System.out.println("继承了Monkey父类");
		Monkey mo=new Monkey();
		mo.jump();
		LittleMonkey li=new LittleMonkey();
		li.swimming();
		li.fly();
	}
}
//接口Fish
interface Fish{
	public void swimming();
}
//接口Bird
interface Bird{
	public void fly();
}
//建立Monkey类
class Monkey{
	int name;
	//猴子可以跳
	public void jump(){
		System.out.println("猴子会跳!");
	}
}
//建立LittleMonkey子类并继承了Monkey父类并连接了Fish和Bird接口
class LittleMonkey extends Monkey implements Fish,Bird{
	public void swimming() {
		System.out.println("连接了Fish接口!");
	}
	public void fly() {
		System.out.println("连接了Bird接口!");
	}
}
-------------------------------------------------------------------------------
用接口实现多态--案例[Demo127.java]
java中多态是个难以理解的概念，但同时又是一个非常重要的概念。java三大特性之一(继承，封装，多态)，我们可以从字面上简单理解：就是一种类型的多种状态，以下通过卖小汽车的例子说明什么是多态。
//用接口实现多态
public class Demo127 {
	public static void main(String []args){
		CarShop aShop=new CarShop();
		//卖出一辆宝马
		aShop.sellCar(new BMW());
		//卖出一辆奇瑞QQ
		aShop.sellCar(new CheryQQ());
		//卖出一辆桑塔纳
		aShop.sellCar(new Santana());
		System.out.println("总收入："+aShop.getMoney());
	}
}
//汽车接口
interface Car{
	//汽车名称
	String getName();
	//获得汽车售价
	int getPrice();
}
//宝马
class BMW implements Car{
	public String getName(){
		return "BMW";
	}
	public int getPrice(){
			return 300000;
	}
}
//奇瑞QQ
class CheryQQ implements Car{
	public String getName(){
		return "CheryQQ";
	}
	public int getPrice(){
		return 20000;
	}
}
//桑塔纳汽车
class Santana implements Car{
	public String getName(){
		return "Santana";
	}
	public int getPrice(){
		return 80000;
	}
}
//汽车出售店
class CarShop{
	//售车收入
	private int money=0;		
	//卖出一部车
	public void sellCar(Car car){
		System.out.println("车型："+car.getName()+"单价："+car.getPrice

());
		//增加卖出车售价的收入
		money+=car.getPrice();
	}
	//售车总收入
	public int getMoney(){
		return money;
	}
}
运行结果：
车型：BMW 单价：300000
车型：CheryQQ 单价：20000
总收入：320000

继承是多态得以实现的基础。从字面上理解，多态就是一种类型(都是Car类型)表现出多种状态(宝马汽车的名称是BMW，售价是300000；奇瑞汽车的名称是CheryQQ，售价是2000)。将一个方法调用同这个方法所属的主体(也就是对象或类)关联起来叫做绑定，分前期绑这下和后期绑定两种。下面解释一下它们的定义：
1、前期绑定：在程序运行之前进行绑定，由编译器和连接程序实现，又叫做静态绑定。比如static方法和final方法，注意，这里也包括private方法，因为它是隐式final的。
2、后期绑定：在运行时根据对象的类型进行绑定，由方法调用机制实现，因此又叫做动态绑定，或者运行时绑定。除了前期绑定外的所有方法都属于后期绑定。

多态就是在后期绑定这种机制上实现的。多态给我们带来的好处是消除了类之间的偶合关系，使程序更容易扩展。比如在上例中，新增加一种类型汽车的销售。只需要让新定义的类实现Car类并实现它的所有方法，而无需对原有代码做任何修改，CarShop类的sellCar(Car
car)方法就可以处理新的车型了。
新增代码如下：
java代码
//桑塔纳汽车
class Santana implements Car{
	public String getName(){
		return "Santana";
	}
	public int getPrice(){
		return 80000;
	}
}
-------------------------------------------------------------------------------
java面向对象编程(3)--final
final概念
final中文意思：最后的，最终的。
final可以修饰变量或者方法。
在某些情况下，程序员可能有以下需求：
1、当不希望父类的某个方法被子类覆盖(override)时，可以用final关键字修饰。
2、当不希望类的某个变量的值被修改，可以用final修饰。如果一个变量是final，则必须赋初值，否则编译出错。
3、当不希望类被继承时，可以用final修饰。
//final方法的使用[Demo128.java]
public class Demo128 {
	public static void main(String[] args) {
		Aaa aaa=new Aaa();
		aaa.show();
		Bbb bbb=new Bbb();
		bbb.show();
	}
}
class Aaa{ 
	int a=0;//如果a不赋初值,a是0。定义类型后应赋值
	//圆周率不让修改
	//带有final修饰的变量命名时应有_下划线来区分表示。这是java程序员的标准。
	final float reate_1=3.1415926f;//使用final可以保证，需要强制不被修改的数据一定要用final锁定
	//final int b;  //使用final定义变量时一定要赋初值否则报错。
	//b=1;
	final public void sendMes(){//给成员方法用final来修饰则表示不可以被修改，不可被覆盖。
		System.out.println("发送消息");
	}
	public void show(){
		System.out.println("a="+a);
	}
}
final class Bbb extends Aaa{//定义类前加final表示该类不允许被继承
	public Bbb(){
		a++;
		//reate_1=reate+1;
	}
	/*public void sendMes(){
		System.out.println("发送消息")
	}*/
}

final--注意事项
1、final修饰的变量又叫常量，一般用XX_XX_XX来命名。(带下划线)
2、final修饰的变量在定义时，必须赋值，并且以后不能再赋值。

final--什么时候用
1、因为案例的考虑，类的某个方法不允许修改。
2、类不会被其它的类继承。
3、某些变量值是固定不变的，比如圆周率3.1415926

 
*******************************************************************************
作业：
第一题：目的
1、变量定义、初始化、赋值
2、运算符和表达式
3、输出语句System.out.println();
 1.作一个加法器，计算它们的和
 2.作一个减法器，计算它们的差
 3.作一个乘法器，计算它们的积
 4.作一个除法器，计算它们的商(和余数)
[Work01.java]
public class Work01{
	public static void main(String []args){
		int i=9;int j=4;
		int k=i+j;
		int l=i-j;
		int m=i*j;
		int n=i/j;
		int o=i%j;
		System.out.println("和："+k+" 差："+l+" 积:"+m+" 商:"+n+" 模："+o);
	}
}
*******************************************************************************
第二题：正方型[Work02.java]
//正方形
public class Work02{
	public static void main(String []args){
		for(int i=1;i<5;i++){
			System.out.println("********");
		}
	}
}
*******************************************************************************
第三题：直角三角形[Work03.java]
//直角三角形
public class Work03{
	public static void main(String []args){
		for(int i=1;i<9;i++){
			for(int j=1;j<i;j++){
				System.out.print("*");
			}
			System.out.println();
		}
	}
}
*******************************************************************************
第四题：三角形[Work04.java]
//三角形
public class Work04{
	public static void main(String []args){
		int lay=10;//行数
		for(int i=1;i<=lay;i++){//循环行
			for(int k=1;k<=lay-i;k++){//找空格
				System.out.print(" ");
			}
				for(int j=1;j<=(i-1)*2+1;j++){//找星位置并输入
					System.out.print("*");
				}
			System.out.println();//换行
		}
	}
}
*******************************************************************************
第五题：
已知手掌游戏机一台320元，MP3一台260元。公司举行抽奖大会，公司有18人，一等奖游戏机，二等奖MP3，购入5公游戏机，13台MP3。问总价为多少，公司实际平均给每人花费多少钱。[Work05.java]
//计算总费用和平均费用
import java.util.*;//加载包
public class Work05{
	public static int gbGame=320;//静态变量
	public static int gbGameT=5;
	public static int mp3=260;
	public static int mp3T=13;
	public static int people=18;
	public static void main(String []args){
		Scanner myScanner=new Scanner(System.in);//调用键盘输入
		showInfo(); //调用showInfo方法
		System.out.print("请输入手掌游戏机价格：");
		gbGame=myScanner.nextInt();
		System.out.print("请输入MP3价格：");
		mp3=myScanner.nextInt();
		System.out.print("请输入手掌游戏机数量：");
		gbGameT=myScanner.nextInt();
		System.out.print("请输入MP3数量：");
		mp3T=myScanner.nextInt();
		showInfo();
		}
	public static void showInfo(){ // 建立showInfo方法
		int total=gbGame*gbGameT+mp3*mp3T;//总价
		float average=(float)total/people;//平均价
		System.out.printf("总价： %d,平均价是: %f \n",total,average);
	}
}
*******************************************************************************
第六题
手掌游戏机一台X元，mp3一台Y元(X,Y,N,M,Z由用户输入)
公司举行抽奖大会，一等奖游戏机N台，二等奖mp3 M台。公司共有Z人。问总价为多少，公司实际平均给每人花费了多少钱。
//计算总费用和平均费用
import java.util.*;//加载包
public class Work06{
	public static int gbGame=0;//静态变量
	public static int gbGameT=0;
	public static int mp3=0;
	public static int mp3T=0;
	public static int people=0;
	public static void main(String []args){
		Scanner myScanner=new Scanner(System.in);//调用键盘输入
		System.out.print("请输入手掌游戏机价格：");
		gbGame=myScanner.nextInt();
		System.out.print("请输入MP3价格：");
		mp3=myScanner.nextInt();
		System.out.print("请输入手掌游戏机数量：");
		gbGameT=myScanner.nextInt();
		System.out.print("请输入MP3数量：");
		mp3T=myScanner.nextInt();
		System.out.print("请输入员工数：");
		people=myScanner.nextInt();
		showInfo();//调用showInfo方法
		}
	public static void showInfo(){ // 建立showInfo方法
		int total=gbGame*gbGameT+mp3*mp3T;//总价
		float average=(float)total/people;//平均价
		System.out.printf("总价： %d,平均价是: %f \n",total,average);
	}
}
*******************************************************************************
第七题
九九乘法表，要求行列对齐[Work07.java]
//九九乘法表
import java.util.*;//加载包
public class Work07{
	public static void main(String []args){
		Scanner myScanner=new Scanner(System.in);//调用键盘输入
		System.out.print("请输入1-9中的一个数：");
		int num=myScanner.nextInt();
		for(int i=1;i<=num;i++){
			for(int j=1;j<=i;j++){
				System.out.print(i+"×"+j+"="+(i*j)+"\t");
			}
		System.out.println();
		}
	}
}
*******************************************************************************
第八题
请使用三个整型变量完成如下功能：
1、用户输入两个整数值；3 5
2、计算两数的和，输出此和； 8
3、求出两数的平均数，输出平均数(整数即可)； 4
4、求出平均数>第二个数的关系表达式的值，输出此值； 0
5、用第一个数减去上面关系表达式的值，得到它们的差，输出差； 3
6、存储第二个数的变量累乘上式的结果，输出此变量的当前值； 15
7、存储第一个数的变量累加第二个变量，输出第一个变量的当前值。 18
//输入两个数完成任务集合[Work08.java]
import java.util.*;//加载包
public class Work08{
	public static void main(String []args){
		Scanner myScanner=new Scanner(System.in);//调用键盘输入
		System.out.print("请输入一个数A：");
		int a=myScanner.nextInt();
		System.out.print("请输入一个数B：");
		int b=myScanner.nextInt();
		int e=0;//定义变量
		//求和	
		int c=a+b;
		System.out.println("和："+c);
		//求平均数
		int d=(a+b)/2;
		System.out.println("平均数："+d);
		//判断平均数是否大于第二个数
		if(d>b){ 
			e=1;
			System.out.println("平均数>第二个数"); 
		}else{
			e=0;
		 	System.out.println("小于"+b+"输出判断值"+e);
		}
		//第一个数减去上式的值
		int f=a-e;
		System.out.println("第一个数减去上式的值"+f);
		//第二个数乘上式的值
		int g=b*f;
		System.out.println("第二个数累乘上式的值"+g);
		//第一个数累加并赋给第一个数
		a+=g;
		System.out.println("第一个数累加第二个数赋给第一个数的值"+a);
	}
}
*******************************************************************************
第九题
渔夫出海打鱼，收获若干
1、渔夫卖掉一半的鱼，然后送给海伦3条；
2、渔夫又卖掉剩下的鱼的2/3，自己吃掉1条；
3、海伦来看渔夫，问他那天打了多少鱼，渔夫数了数，还剩4条鱼，渔夫对海伦怎么说？
//打鱼--共有多少鱼[Work09.java]
public class Work09{
	public static void main(String []args){
		int total=0;
		int rest=4;//剩余的鱼
		total=((rest+1)*3+3)*2;//逆推
		System.out.println("鱼一共有："+total);
	}
}
*******************************************************************************
第十题
有一只猴子摘了一堆桃子，当即吃了一半，可是桃子太好吃了，它又多吃了一个，第二天它把第一天剩下的桃子吃了一半，又多吃了一个，就这样到第十天早上它只剩下一个桃子了，问它共摘了多少桃子[Work10.java]
import java.util.*;//加载包
public class Work10{
	public static void main(String []args){
		Monkey mo=new Monkey();
		mo.scan();
	}
}
class Monkey{
	//day哪天的桃子数，sday吃了多少天剩下一个
	public static int peach(int day,int sday){//建一个peach方法
		if(day==sday){
			return 1;
		}else{
			return (peach(day+1,sday)+1)*2;//算法返回值
		}
	}
	public static void scan(){ //建立输入的方法
		int a=1;
		System.out.println("请输入要吃几天：");
		Scanner sr=new Scanner(System.in);
		int b=sr.nextInt();
		if(a<b){
			System.out.print(Monkey.peach(a,b));
		}else{
			System.out.println("不能小于等于1天");
			Monkey.scan();
		}
	}
}
*******************************************************************************
第十一题
计算1+2+3+...+20=?思考如果让用户输入一个整数n计算累加和：1+2+3+...+n能做到吗？
[Work11.java]
import java.util.*;//加载包
public class Work11{
	public static void main(String []args){
		Scanner myScanner=new Scanner(System.in);//调用键盘输入
		System.out.print("请输入一个数N：");
		int n=myScanner.nextInt();
		int i=0;
		for(int m=0;m<n;m++){
			i=i+(m+1);
			System.out.println("m是"+m);
		}
		System.out.println("1+2+3+...+n的值是"+i);	
	}
}
*******************************************************************************
第十二题
请编写一个Cat类，要求如下：
该猫可以做四则运算，也可以进行面积计算；
将四则运算器和面积运算器合二为一，作一个运算器，主菜单让用户选择是做四则运算还是面积运算，分为两个子菜单，让用户选择加减乘除或者形状。
//一个Cat类进行四则运算和面积计算[Work12.java]
//一个Cat类进行四则运算和面积计算
import java.util.*;//加载包
public class Work12{
	public static void main(String []args){
		Cat cat=new Cat();
		cat.scan1();
	}
}
class Cat{
	//输入方法
	public static void scan1(){
		System.out.println("题目类型如下");
		System.out.println("1、四则运算");
		System.out.println("2、面积运算");
		System.out.println("0、退出程序");
		System.out.print("请选择要做题的类型，请入0-2：");
		Scanner sr=new Scanner(System.in);
		int x=sr.nextInt();
		switch(x){
			case 0:
				System.out.println("谢谢使用，再见!");//退出
				break;
			case 1:
				Cat.szys();
				break;
			case 2:
				Cat.mjys();
				break;
			default:
				System.out.println("输入有误，请重新输入!");
			Cat.scan1();//重复调用目录
		}
	}
	//四则运算方法
	public static void szys(){
			System.out.println("四则运算");
			System.out.println("1、加法运算");
			System.out.println("2、减法运算");
			System.out.println("3、乘法程序");
			System.out.println("4、除法程序");
			System.out.println("0、返回上级");
			System.out.print("请选择要做题的类型，请入0-4：");
			Scanner sr=new Scanner(System.in);
			int y=sr.nextInt();
			switch(y){
				case 0:
					System.out.println("返回上级");
					Cat.scan1();//调用主目录
					break;
				case 1:
					System.out.println("进入加法运算，请输入第一个数：");
					Scanner jf1=new Scanner(System.in);
					int jf01=jf1.nextInt();
					System.out.println("进入加法运算，请输入第二个数：");
					Scanner jf2=new Scanner(System.in);
					int jf02=jf2.nextInt();
					float jfh=(float)jf01+(float)jf02;
					System.out.println(jf01+"+"+jf02+"="+jfh);
					System.out.println("已计算完成。");
					System.out.println("是否要继续使用？使用请输入1，返回请输入2，退出请输入任意数字:");
					Scanner cz01=new Scanner(System.in);
					int cz001=cz01.nextInt();
					if(cz001==1){
						Cat.szys();
					}else if(cz001==2){
						Cat.scan1();
					}else if(cz001!=1||cz001!=2){
						System.out.println("谢谢使用，再见!");
					}
					break;					
				case 2:
					System.out.println("进入减法运算，请输入第一个数：");
					Scanner jjf1=new Scanner(System.in);
					int jjf01=jjf1.nextInt();
					System.out.println("进入减法运算，请输入第二个数：");
					Scanner jjf2=new Scanner(System.in);
					int jjf02=jjf2.nextInt();
					float jjfh=(float)jjf01-(float)jjf02;
					System.out.println(jjf01+"-"+jjf02+"="+jjfh);
					System.out.println("已计算完成。");
					System.out.println("是否要继续使用？使用请输入1，返回请输入2，退出请输入任意数字:");
					Scanner cz02=new Scanner(System.in);
					int cz002=cz02.nextInt();
					if(cz002==1){
						Cat.szys();
					}else if(cz002==2){
						Cat.scan1();
					}else if(cz002!=1||cz002!=2){
						System.out.println("谢谢使用，再见!");
					}
					break;
				case 3:
					System.out.println("进入乘法运算，请输入第一个数：");
					Scanner cff1=new Scanner(System.in);
					int cff01=cff1.nextInt();
					System.out.println("进入乘法运算，请输入第二个数：");
					Scanner cff2=new Scanner(System.in);
					int cff02=cff2.nextInt();
					float cffh=(float)cff01*(float)cff02;
					System.out.println(cff01+"×"+cff02+"="+cffh);
					System.out.println("已计算完成。");
					System.out.println("是否要继续使用？使用请输入1，返回请输入2，退出请输入任意数字:");
					Scanner cz03=new Scanner(System.in);
					int cz003=cz03.nextInt();
					if(cz003==1){
						Cat.szys();
					}else if(cz003==2){
						Cat.scan1();
					}else if(cz003!=1||cz003!=2){
						System.out.println("谢谢使用，再见!");
					}
					break;
				case 4:
					System.out.println("进入除法运算，请输入第一个数：");
					Scanner cf1=new Scanner(System.in);
					int cf01=cf1.nextInt();
					System.out.println("进入除法运算，请输入第二个数：");
					Scanner cf2=new Scanner(System.in);
					int cf02=cf2.nextInt();
					float cfh=(float)cf01/(float)cf02;
					System.out.println(cf01+"÷"+cf02+"="+cfh);
					System.out.println("已计算完成。");
					System.out.println("是否要继续使用？使用请输入1，返回请输入2，退出请输入任意数字:");
					Scanner cf03=new Scanner(System.in);
					int cf003=cf03.nextInt();
					if(cf003==1){
						Cat.szys();
					}else if(cf003==2){
						Cat.scan1();
					}else if(cf003!=1||cf003!=2){
						System.out.println("谢谢使用，再见!");
					}
					break;
				default:
					System.out.println("输入有误，请重新输入!");
				Cat.szys();//循环调用子目录
			}
		}
	//面积运算方法
	public static void mjys(){
			System.out.println("面积运算");
			System.out.println("1、三角形面积计算");
			System.out.println("2、圆形面积计算");
			System.out.println("3、方形面积计算");
			System.out.println("0、返回上级");
			System.out.print("请选择要做题的类型，请入0-3：");
			Scanner sr=new Scanner(System.in);
			int z=sr.nextInt();
			switch(z){
				case 0:
					System.out.println("返回上级");
					Cat.scan1();//调用主目录
					break;
				case 1:
					System.out.println("进入三角形面积计算，请输入底：");
					Scanner sj1=new Scanner(System.in);
					int sjx01=sj1.nextInt();
					System.out.println("进入三角形面积计算，请输入高：");
					Scanner sj2=new Scanner(System.in);
					int sjx02=sj2.nextInt();
					float sjxh=((float)sjx01*(float)sjx02)/2;
					System.out.println("底"+sjx01+" 高："+sjx02+" 面积="+sjxh);
					System.out.println("已计算完成。");
					System.out.println("是否要继续使用？使用请输入1，返回请输入2，退出请输入任意数字:");
					Scanner sj03=new Scanner(System.in);
					int sj003=sj03.nextInt();
					if(sj003==1){
						Cat.mjys();
					}else if(sj003==2){
						Cat.scan1();
					}else if(sj003!=1||sj003!=2){
						System.out.println("谢谢使用，再见!");
					}
					break;
				case 2:
					System.out.println("进入圆形面积计算，请输入半径：");
					Scanner y1=new Scanner(System.in);
					int bj=y1.nextInt();
					float ymjh=(float)bj*(float)bj*3.1415926f;
					System.out.println("半径:"+bj+" 面积:"+ymjh);
					System.out.println("已计算完成。");
					System.out.println("是否要继续使用？使用请输入1，返回请输入2，退出请输入任意数字:");
					Scanner y01=new Scanner(System.in);
					int y001=y01.nextInt();
					if(y001==1){
						Cat.mjys();
					}else if(y001==2){
						Cat.scan1();
					}else if(y001!=1||y001!=2){
						System.out.println("谢谢使用，再见!");
					}
					break;
				case 3:
					System.out.println("进入方形面积计算，请输入长：");
					Scanner c1=new Scanner(System.in);
					int c01=c1.nextInt();
					System.out.println("进入方形面积计算，请输入宽：");
					Scanner k2=new Scanner(System.in);
					int k02=k2.nextInt();
					float mjh=(float)c01*(float)k02;
					System.out.println("长:"+c01+" 宽："+k02+" 面积:"+mjh);
					System.out.println("已计算完成。");
					System.out.println("是否要继续使用？使用请输入1，返回请输入2，退出请输入任意数字:");
					Scanner m03=new Scanner(System.in);
					int m003=m03.nextInt();
					if(m003==1){
						Cat.mjys();
					}else if(m003==2){
						Cat.scan1();
					}else if(m003!=1||m003!=2){
						System.out.println("谢谢使用，再见!");
					}
					break;
				default:
					System.out.println("输入有误，请重新输入!");
				Cat.mjys();//循环调用子目录
			}
		}
}
*******************************************************************************
第十三题
请大家采用面向对象思想设计超级马里奥游戏人物。并能用键盘输入命令，来控制马里奥的位置[Work13.java]
//超级马里奥人物建造及控制台数字操作
import java.util.*;
public class Work13 {
	public static void main(String[] args) {
		Scanner sr=new Scanner(System.in);//接收键盘输入
		System.out.println("输入1-25的数字，你可以移动马里奥，输入其它数字退出");
		int i=sr.nextInt();//将键盘输入数字赋值给i
		Maria m=new Maria();//建立调用Maria构造方法
		for(int a=i;a<=25;a--){
			if(i<25){
				m.move(i);
				i=sr.nextInt();
			}else{
				System.out.println("退出游戏!");
				break;
			}
		}
	}
}

class Maria{
	int x,y;
	//构造方法，初始化场景；确定地图，Maria的位置
	public Maria(){
		System.out.println("I'm Maria \n"+"@");
	}
	public void move(int i){
		for(int k=1;k<=25;k++){
			if(k==i){
				System.out.printf("@");
			}else{
				System.out.printf(".");
			}
		}
	}
}
*******************************************************************************
代码分析：
1、运行一下代码，将得到什么打印结果：
int i=3;
int j=0;
double k=3.2;
if(j<k)
if(i==j)
System.out.println(i);
else
System.out.println(j);//执行此语句，得到结果0
else
System.out.println(k);
-------------------------------------------------------------------------------
2、以下代码能否编译通过？假如能编译通过，运行时得到什么打印结果？
int i=4;
switch(i){
	default;
	System.out.println("default");//执行此语句
case 0:
	System.out.println("zero");//执行此语句
break;
case 1:
System.out.println("one");
case 2:
System.out.println("two");
}
-------------------------------------------------------------------------------
3、以下那些代码是合法的？
a)
int i;
for(i=5,int j=10;i<10;j--){}//错
b)
int i,j;
for(i=0,j=10;i<10,j>0;i++,j--){}//错
c)
int i,k;
for(i=0,k=9;(i<10&&k>0);i++,j--){}//错
d)
int i,j
for(i=0;j=10;i<10;i++,j--){}//错
-------------------------------------------------------------------------------
4、运行以下代码，将得到什么打印结果？
int i=1;
switch(i){
default:
System.out.println("default");
case 0:
System.out.println("zero");
break;
case 1;
System.out.println("one");//执行此语句
case2;
System.out.println("two");//执行此语句
}
-------------------------------------------------------------------------------
5、以下代码是合法的？
a)
float x=1;//数据类型错误
switch(x){
case 1:
System.out.println("Got a 1");//错
}
b)
long y=1;//数据类型错误
switch(y){
case 1:
System.out.println("Got a 1");//错
}
c)
byte x=1;//低精转高精
switch(x){
case 1/1:
System.out.println("Got a 1");//正确
}
d)
int x=1;
int c=1;
switch(c){
case x;//需常量
System.out.println("Got a 1");//错
break;
e)
short x=1;//数据类型错误
switch(x){
case 3.2/3:
System.out.println("Got a 1");
break;
}
f)
shout x=1;//数据类型错误
switch(x){
case 1,2,3:
System.out.println("Got a 1");//错
break;
}
-------------------------------------------------------------------------------
6、以下代码能否编译通过？假如能编译通过，运行时将得到什么打印结果？
public class Myswitch{
	public static void main(String args[]){
		Myswitch ms=new Myswitch();
		ms.amethod();
	}
	public void amethod(){
		for(int a=0,b=0;a<2;b=++a,System.out.println("b="+b)){
			System.out.println("a="+a);
		}
	}
}
结果：a=0
      b=1
      a=1
      b=2
-------------------------------------------------------------------------------
7、以下代码能否编译通过？假如能编译通过，运行时将得到什么打印结果？
void looper(){
	int x=0;
	one:
	while(x<10){
		two:
		System.out.println(++x);
		if(x>3)
		break two;
	}
}//无法编译，break two;无法返回到two标签
-------------------------------------------------------------------------------
8、以下代码能否编译通过？假如能编译通过，运行时将得到什么打印结果？
public class Hope{
	public static void main(String args[]){
		Hope h=new Hope();
	}
	protected Hope(){
		int i=1;
		do{
		System.out.println(i);
		}while(++i<3);
	}
}
结果：1 2
*******************************************************************************
第十四题
请编写一个猜拳的游戏
有个人Tom设计他的成员变量，成员方法，可以电脑猜拳。电脑每次都会随机生成0,1,2；0表示石头、1表示剪刀、2表示布
//与电脑猜拳[Work14_1.java]
import java.util.*;
public class Work14_1 {
	public static void main(String[] args) {
			Kais.jingcyx();//调用开始游戏
	}
}
//开始退出游戏类
class Kais{
	public static void jingcyx(){
		System.out.println("是否开始猜拳游戏？按1开始，按0退出");
		Scanner sr=new Scanner(System.in);
		int x=sr.nextInt();
		switch (x){
			case 0:
				System.out.println("已退出游戏!");	
				break;
			case 1:
				System.out.println("游戏说明：0代表石头，1代表剪刀，2代表布");
				Caiquan.caiquan();
				break;
			default:
				System.out.println("输入错误，请重新输入!");
				Kais.jingcyx();
				break;
		}
	}
}
//猜拳游戏
class Caiquan{
	public static void caiquan(){
		int a1=0,b1=0,c1=0;
		System.out.print("请输入想玩的盘数：");
		Scanner p=new Scanner(System.in);
		int ps=p.nextInt();
		for(int i=1;i<=ps;i++){
			System.out.println("游戏已开始，请出拳!");
			Scanner m=new Scanner(System.in);
			int a=m.nextInt();//玩家出拳
			//Random n=new Random(2);//随机函数
			int b=(int)(0+Math.random()*(3-1+1));//随机产生0-2的int数，电脑出拳
			if(a==b){
				a1++;
				System.out.println("打平!");
			}else if((a-b)==-1||(a-b)==2){
				b1++;
				System.out.println("YOU Win!");
			}else{
				c1++;
				System.out.println("YOU LOSE");
			}
		}
		System.out.println("平:"+ a1 +"\n赢:" + b1 +"\n输:"+c1+"\n一共玩了"+(a1+b1+c1)+"局");
		Kais.jingcyx();
	}
}
*******************************************************************************
第十五题
请编写一个类koradji(巫师的意思)
为类编写如下功能：
1、根据用户的输入某人的生日，可以计算出该人的星座；
2、根据用户的输入年月日可以计算是星期几；
3、可以显示该巫师给多少人算过星相。
 1月20日- 2月18日水瓶  2月19日- 3月20日双鱼  3月21日- 4月19日白羊
 4月20日- 5月20日金牛  5月21日- 6月20日双子  6月21日- 7月22日巨蟹
 7月23日- 8月22日狮子  8月23日- 9月22日处女  9月23日-10月22日天秤
10月23日-11月21日天蝎 11月22日-12月21日射手 12月22日- 1月19日摩羯
//通过输入生日显示出生在周几。巫师看星座[Wrok15.java]
import java.util.*;
public class Work15{
	public static void main(String []args){ //程序入口
		Start ks=new Start();//调用程序开始类Start，并启用st方法
		ks.st();
	}
}

class Start{//程序开始类
	public void st(){
		System.out.println("年月日格式：19XX XX XX\n请输入出生年月日：");
		Scanner sr=new Scanner(System.in);
		int year=sr.nextInt();//输入年
		int month=sr.nextInt();//输入月
		int date=sr.nextInt();//输入日
		Rq r=new Rq();	//调用周几类
		r.rq(year,month,date);//将年月日数据传给周几类的rq方法中
		Xinz xz=new Xinz();//调用星座类
		xz.xinz(month,date);//将月日的数据传给星座类中的xinz方法中
		System.out.println("\n是否继续让巫师看星座？\n1、继续\t2、退出");
		Scanner sr1=new Scanner(System.in);
		int o=sr1.nextInt();
		if(o==1){
			Start qd=new Start();//输入1调用程序开始类
			qd.st();
		}else if(o!=1){	//不等于1退出
			Xinz tc=new Xinz();
			System.out.println("巫师为"+tc.getI()+"人看过星座");
			System.out.println("退出星座查询，Goodbay!");
		}
	}
}

class Rq{//周几类
	public void rq(int year,int month,int date){
		Calendar c = Calendar.getInstance(); //调用日期Calendar抽象类
		c.set(Calendar.YEAR,year);	
		c.set(Calendar.MONTH,month-1);
		c.set(Calendar.DATE,date);
		int week = c.get(Calendar.DAY_OF_WEEK);
		switch (week){ //判断输入的日期是周几
		case 1:
			System.out.println("星期日");
			break;
		case 2:
			System.out.println("星期一");
			break;
		case 3:
			System.out.println("星期二");
			break;
		case 4:
			System.out.println("星期三");
			break;
		case 5:
			System.out.println("星期四");
			break;
		case 6:
			System.out.println("星期五");
			break;
		case 7:
			System.out.println("星期六");
			break;
		}
	}
}

class Xinz{ //星座类
	public static int i=0;//定义静态变量i，i为统计调用人数计数器
	public void xinz(int month,int date){ //判断星座的方法
	i++;//调用此方法计数累器
		switch(month){
			case 1:{
				if(date>=20){
					System.out.println("水瓶座");
				}else{
					System.out.println("摩羯座");
				}
				break;
			}
			case 2:{
				if(date>=19){
					System.out.println("双鱼座");
				}else{
					System.out.println("水瓶座");
				}
				break;
			}
			case 3:{
				if(date>=21){
					System.out.println("白羊座");
				}else{
					System.out.println("双鱼座");
				}
				break;
			}
			case 4:{
				if(date>=20){
					System.out.println("金牛座");
				}else{
					System.out.println("白羊座");
				}
				break;
			}
			case 5:{
				if(date>=21){
					System.out.println("双子座");
				}else{
					System.out.println("金牛座");
				}
				break;
			}
			case 6:{
				if(date>=21){
					System.out.println("巨蟹座");
				}else{
					System.out.println("金牛座");
				}
				break;
			}
			case 7:{
				if(date>=23){
					System.out.println("狮子座");
				}else{
					System.out.println("巨蟹座");
				}
				break;
			}
			case 8:{
				if(date>=20){
					System.out.println("处女座");
				}else{
					System.out.println("巨蟹座");
				}
				break;
			}
			case 9:{
				if(date>=23){
					System.out.println("天平座");
				}else{
					System.out.println("处女座");
				}
				break;
			}
			case 10:{
				if(date>=23){
					System.out.println("天蝎座");
				}else{
					System.out.println("天平座");
				}
				break;
			}
			case 11:{
				if(date>=22){
					System.out.println("射手座");
				}else{
					System.out.println("天蝎座");
				}
				break;
			}
			case 12:{
				if(date>=22){
					System.out.println("摩羯座");
				}else{
					System.out.println("射手座");
				}
				break;
			}
		}
	}
	public int getI(){ //返回统计调用次数
		return i;
	}
}

*******************************************************************************
 

第十六题
10个人投票选班长，有三个侯选人(张三，李四，王五)，通过编号投票，要求最后显示班长姓名。[Work16.java]
import java.util.*;
public class Work16 {
	public static void main(String[] args) {
		//设定投票人数
		System.out.print("设定投票人数：");
		Scanner sr=new Scanner(System.in);
		int a=sr.nextInt();
		System.out.print("请输入第1位侯选人的名字：\n");
		Scanner sr1=new Scanner(System.in);
		String i1=sr1.nextLine();//键盘接收字符串
		System.out.print("请输入第2位侯选人的名字：\n");
		Scanner sr2=new Scanner(System.in);
		String i2=sr2.nextLine();
		System.out.print("请输入第3位侯选人的名字：\n");
		Scanner sr3=new Scanner(System.in);
		String i3=sr3.nextLine();
		System.out.println("本次选举将有"+ a +"人参与!");
		System.out.println("1号:"+i1+"\t2号:"+i2+"\t3号:"+i3);
		Xuanju tp=new Xuanju();
		tp.tp(a,i1,i2,i3);
	}
}
class Xuanju{
	public void tp(int a,String i1,String i2,String i3){
		int j1=0,j2=0,j3=0,qq=0;//计票器
		for (int i=1;i<=a;i++){ //统计投票
			System.out.println("请投票，投票请按1,2,3：");
			Scanner tp=new Scanner(System.in);
			int b=tp.nextInt();
			System.out.println("已有"+ i +"人投票");
			switch (b){
				case 1:
					j1++;
					break;
				case 2:
					j2++;
					break;
				case 3:
					j3++;
					break;
				default:
					qq++;
					break;
			}
		}
		
		if(j1>j2&&j1>j3){
			System.out.println(i1 +"得"+ j1 +"票\n"+ i2 +"得"+ j2 +"票\n"+ i3 +"得"+ j3 +"票\n"+"弃权票数"+qq);
			System.out.println("恭喜" + i1 + "当选班长!");
		}else if(j1<j2&&j2>j3){
			System.out.println(i1 +"得"+ j1 +"票\n"+ i2 +"得"+ j2 +"票\n"+ i3 +"得"+ j3 +"票\n"+"弃权票数"+qq);
			System.out.println("恭喜" + i2 + "当选班长!");
		}else if(j3>j1&&j2<j3){
			System.out.println(i1 +"得"+ j1 +"票\n"+ i2 +"得"+ j2 +"票\n"+ i3 +"得"+ j3 +"票\n"+"弃权票数"+qq);
			System.out.println("恭喜" + i3 + "当选班长!");
		}else {
			System.out.println(i1 +"得"+ j1 +"票\n"+ i2 +"得"+ j2 +"票\n"+ i3 +"得"+ j3 +"票\n"+"弃权票数"+qq);
			System.out.println("有同等票数，投票无效重新投票!");
		}
	}
}