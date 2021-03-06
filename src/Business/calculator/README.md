# 算式计算器
**欢迎加入商业平台学院QQ群38234781，获得与导师一对一的沟通机会**

## 任务目的
* 对于程序员来说，使用那种“归零归零归零”的按键式计算器多数情况下是不爽的。
* 我们更喜欢一个能直接输入算式的计算器。
* 同时，现有科学计算器的功能是很落后，主要是便宜的计算器不支持编程操作，即使能编程，实现的功能也是很弱的。我们希望得到一个编程功能稍微强大一点儿的计算器。

## 任务描述
* 首先，我们需要一个能输入算式的计算器
    * 算式以文本的形式输入，输入后，通过一个按钮执行计算，给出计算结果。
    * 这个计算器只有文本输入框和一个计算按钮。
    * 我们不希望你使用eval或者new Function的方式把输入的算式转换成代码直接执行，除非你能正确的替换输入中的数学运算符和常用函数名称，并阻挡住所有的注入攻击。
    * 计算器应当能支持以下运算：
        * +: 加法运算
        * -: 减法运算
        * *: 乘法运算
        * /: 除法运算
        * ^: 乘方运算，2 ^ 3 = 8
        * %: 取余运算，3 % 2 = 1
        * abs: 绝对值运算，abs(-1) = 1
        * avg: 均值运算，avg(1,2) = 1.5
        * sin: 正弦运算，sin(30) = 0.5
        * cos: 余弦运算，cos(60) = 0.5
        * tan: 正切运算，tan(45) = 1
        * cot: 余切运算，cot(45) = 1
        * log: 取10底对数运算，log(100) = 2
        * ln: 取自然对数运算
        * e: 常量，自然对数
        * π: 常量，代表圆周率
        * 若支持其他运算，请在readme.md中给出，有额外加分

* 其次，我们希望能自定义运算
    * 这个功能类似于自定义函数
    * 只允许一个自定义运算，名字叫MyJob
    * 允许用户输入这个子运算的算式，比如自定义运算要计算立方体体积，用户可以把子运算写成：x1 x2 x3
    * 在主运算中使用自定义运算：MyJob(1, 2, 3) = 6
    * 自定义运算只要求支持上面提到的标准运算，不需要再嵌套自定义运算

* 最后，算式计算器应当有错误的提示
    * 若输入的算式格式不正确，直接给出提示
    * 若计算过程中出现无意义的情况，请直接给出结果"NaN"，意为not a number
    * 若出现无穷的情况，直接给出n+或n-

## 任务注意事项
* 请提交工程在github的托管地址
* **请尽量使用JS原生API开发**，允许使用jQuery等简单框架
* 请合理组织代码结构，添加必要的注释
* 工程以index.html启动，第三方库放在dep文件夹中，项目代码放在src文件夹中
* 如工程需要构建或特殊启动流程，请在readme.md中提供

## 在线学习参考资料
[四则运算表达式求值](http://blog.csdn.net/yzl_rex/article/details/7745341)