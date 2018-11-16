# Clean Code  
—— [美]Robert C.Martin 著 韩磊 译  
—— A handbook of Agile Software Craftsmanship  

Hello, everybody! It's Clare. The book, named 'Clean Code', which I've been touched in with for months. First I'll appreciate my friend :sparkles:***Jason***:sparkles:, the gentleman, who guide me the direction and borrow me the book.  
#### Statement  
I'll update the text whenever I gain some kind of things that made me inspired. The language will be Chinese since the book has been translated to it. Here we go!  

## 命名
1. 要有含义
    1. 避免在变量不是`list`类型的时候用诸如`accountList`命名；
    2. 不同名要明显区分，避免`getActiveAccount()`、 `getActiveAccountData()`和 `getActiveAccountInfo()`同时存在；
    3. 单字母仅用于**短**方法，`i`, `j`, `k`传统惯用循环器；
    4. 选词：
        1. 概念和词一一对应
        2. 避免双关
        3. 可选解决方案/专业领域相关
        4. 创造语境
2. 区分不同场合
    1. 类名：名词/名词短语；
    2. 方法名：动词/动词短语；  
    
*(:expressionless: Forgive me for the impressive logic, What I wrote down is not the entire content. And the order has been modified to suit my own memory.)*    
## 函数
遵循以下两点规则吧：
1. 短
2. 只做一件事
3. 向下规则  
    什么是向下规则，举个例子，运用该规则后可以这样将程序读出来：
    ```
    To include the setups and teardowns, we include setups, then we include the test page content and then we inclued the teardowns.
    To include the setups, we include the suite setup if this is a suite, then we include the regular setup.
    To include the suite setup, we search the parent hierarchy for the "SuiteSetUp" page and add an include statement with the path of that page.
    To search the parent...
    ```
##### 关于函数的输入参数：  
无参数输入最理想  
一元还凑合  
二元读起来费劲，往往会将输入参数的顺序搞混  
三元不可接受  

*减少参数的修正方法：*  
1. 列表（前提是几个输入参数相关）
2. 使用对象:star::star::star:
##### 容易产生误会的几点：
1. 命名产生的误会，做不到看到名字知晓功能
1. 一个转换功能的函数，有参数输入，无参数输出
3. 一个用户交互的函数，返回`Boolean`并出现在`if`语句的判别条件中
4. 一个检查密码是否正确的函数`CheckPassword()`中包含一步**初始化**操作，不明真相的人调用该函数的感受：:broken_heart::broken_heart::broken_heart:
##### 最后改好函数的三点：
1. 分解函数（Smaller）
2. 修改名称（meaning）
3. 消除重复（ function/object）:point_left:这是终极目标
   
OK, 今天就写到这里吧，多实践才可以好好运用规则哦~ 现在要去改代码了。（话说中英文混杂会挨打的，不管了，反正也没人看[捂脸][捂脸]）
Oh, by the way, it's Nov 16th, 2018.
