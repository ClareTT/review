# MATLAB 面向对象编程
——从入门到设计模式（徐 潇   李 远   编著）   
【北京航空航天大学出版社】    
[BEIHANG UNIVERSITY PRESS]    

Hi, everybody! It's a new book. It's Clare who is editing this, obviously. Most importantly, today, is Programmer's Day, again. Remember the ***1024*** last year, i'm uploading some little demo of code which can be carried up in github.    
Not knowing why, i'm totally not in the state of work after *16:00*. I'm not sure whether it was because of the terrible weather or the terrible weather. Oh. What i'm saying is just nonsense. I'm more convinced of the opinion in ***predictably irrational*** that people can not predict one's strategy at their different emotional state. And, one can not make everything to run as he planned beforehand.    
Back to the book, right, first i'll push the catelog... of the first part that i've read of course. The whole catelog is juuust a huge. Ha~    

#### 第 1 部分 面向对象编程初级篇
##### 第1章 面向过程和面向对象程序设计
##### 第2章 MATLAB面向对象程序入门
It seems like the catalog is so boring, let's just not push it.    
好，接下来是中文叙述~    
今天就读了上面两章，不过，还蛮有启发的，MATLAB本身的特点不在于OOP，但是该功能在奥运会那年发布的新版本就已经提供OOP功能了，市面上的语言（Java，C++）基本都有面向对象编程，我的目的还是要通过这本来学习面向对象编程思想的，没想到还大有收获。    
读完的感受，对以下几个事实表示刷新了对OOP的认识。    
1. 构造函数返回值是对象，对象的创建过程实际上是调用的类的构造函数（怪不得二者名字保持一致）；
2. 常量是一种类型，其值不可更改；
3. 如果一个类的成员变量的值需要用其他成员变量计算而来，那么这个变量最好定义为Dependenct属性；    
4. 不想让除了开发者以外的人看到的属性和方法，可以设置其Hidden=true；
5. 类的方法都有一个参数是obj（这只是个代号），在其他语言中，这个参数可能是隐藏的；
6. MATLAB中调用成员方法可以用Dot，也可以（obj，arg1，...），这样；
