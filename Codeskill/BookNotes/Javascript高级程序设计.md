# Javascript 读书笔记
>总共25章

## 1.简介
  * 由三个核心构成
    * 1. ECMAScript（欧洲计算机制造协会European Computer Manufacturers Association），由ECMA-262定义，提供核心语言功能
    * 文档对象模型(DOM,Document Object Model),提供访问和操作网页内容的方法和接口
    * 浏览器对象模型(BOM, Browser Object Model),提供与浏览器的方法与接口

## 2.在HTML中使用Javascript
  * `<script>`元素
    * type="text/javascript"
    * src="./pwd"
    * 还有4个async/charset/defer/language 不常用
  * 标签位置
    * 最好放置body 元素的后面，有助于用户感觉缩短打开时间
  * 延迟 defer
  * 异步脚本 async
## 3.基本概念
  * 语法
    * 区分大小写
    * 标识符号
    * 注释
    * 严格模式
    * 语句
  * 关键字和保留字
  * 变量
  >var 局部变量/全局变量

  * 数据类型
    * typeof操作符
    * underfined类型
      * 声明变量但未对其初始化
    * Null类型
      * 表示空指针
    * boolean类型
      * true  ！=1
      * false ！=0
    * number类型
      * 整数和浮点数
        * 十进制/八进制/十六进制Ox
        * 浮点数
        * 数值范围
        * NaN（Not a Number）
        * 数值转换
          * Number/parentInt/parseFloat
    * string类型
      * 字符字面量/转义字符
      * 转换为字符串 toString
    * Object类型
      * constructor/保存着用于创建当前对象的函数
      * hasOwnProperty/用于检查给定的属性在当前对象实例中是否存在
      * isPrototypeOf/检查传入对象是否是传入对象的原型
      * propertyIsEnumerable/用于检查给定的属性是否能够使用for-in语句来枚举
      * toLocaleString/返回对象的字符串表示，与地区对应
      * toString/返回对象的字符串表示
      * valueOf/ 返回对象的字符串，数值或布尔值表
  * 操作符
    * 一元操作符
      * 递增和递减
      * 一元加和减操作符
    * 位操作符
      * 按位非 not ~
      * 按位与 and &
      * 按位或 or |
      * 按位异或 xor ^
      * 左移 <<
      * 有符号的右移 >>
      * 无符号右移 >>>
    * 布尔操作符
      * 非not!/与and &&/或or ||
    * 乘性操作符
      * 乘法 (* )  /除法 (\ ) /求模 (%)
    * 加性操作符
      * 加法+/减法-
    * 关系操作符
      * 小于 (<) /大于 (>)/小等于 (<=)/大等于(>=)
    * 相等操作符
      * ==
    * 全等和不等
      * ===
      * ！==
    * 条件操作符
    * 赋值操作符
    * 逗号操作符
  * 流控制语句
    * if
    * do-while
    * while
    * for
    * for-in
    * label
    * break/continue
    * with
    * switch
  * 函数
## 4.变量，作用域和内存问题
### 4.1基本类型和引用类型的值
### 4.2 执行环境及作用域
### 4.3 垃圾收集
### 4.4 小结
## 5.引用类型
### 5.1 Object 类型
  * 2种方法创建
### 5.2 Array类型
  * 2种创建方式
  * 如何显示，修改，增加数组
  * 如何显示，修改数组的长度，如果修改了数组的长度，新增加的值默认是什么？
  * 如何检测数组？
  * array如何转换为其他类型？/tolocalestring/tostring/valueOf
  * 转换为字符串的时候如何用|分割对象
  *  数组的栈方法 push/pop
  * 数组的队列方法 shift/unshift
  * 重排序方法？reverse/sort   
  * sort 的比较函数？
  * 
### 5.3 Data类型
### 5.4 RegExp类型
### 5.5 Function类型
### 5.6 基本包装类型
### 5.7 单体内置对象
### 5.8 小结
## 6.面向对象的程序设计
## 7.函数表达式
## 8.BOM
## 9.客户端检测
## 10.DOM
## 11.DOM扩展
## 12.DOM2和DOM3
## 13.事件
## 14.表单脚本
## 15.使用Canvas绘图
## 16.HTML5脚本编程
## 17.错误处理和调试
## 18.Javascript和XML
## 19.E4X
## 20.JSON
## 21.Ajax与Comet
## 22.高级技巧
## 23.离线应用和客户端存储
## 24.最佳实践
## 25.新兴API
