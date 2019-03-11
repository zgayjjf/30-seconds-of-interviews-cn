### JavaScript 里面表达式（Expression）和语句（Statement）的区别是什么？

#### Answer

JavaScript 里面有两个主要的语法类别：表达式和语句。第三种语法是同时使用两者，称为表达式语句（Expression statement）。它们可以大致总结如下：

* **表达式（Expression）**: 产生一个值
* **语句（Statement）**: 执行一个操作
* **表达式语句（Expression statement）**: 产生一个值并且执行一个操作

经验法则:

> 如果你可以打印出来或者把它赋给一个变量，那么他是一个表达式。如果不能，那它是一个语句。

##### Statements

```js
let x = 0

function declaration() {}

if (true) {
}
```

语句执行操作，但是不产生值。

```js
// 将 `y` 的绝对值赋给 `x`
var x
if (y >= 0) {
  x = y
} else {
  x = -y
}
```

上面唯一的表达式是 `y >=0`，它产生了一个值，`true` 或者 `false`。值不是由代码的其他部分产生的。

##### Expressions

表达式产生一个值。他们可以被传到函数里面，因为解释器会用他们解析出来的值替换它们。

```js
5 + 5 // => 10

lastCharacter("input") // => "t"

true === true // => true
```

##### 表达式语句

通过使用条件运算符，可以将之前的语句集转化为一个等价的表达式。

```js
// 将 `y` 的绝对值赋给 `x`
var x = y >= 0 ? y : -y
```

这既是表达式也是语句，因为我们声明了一个变量 `x`（语句），其值为一个求值结果（表达式）

#### Good to hear

* 函数声明和函数表达式

##### Additional links

* [声明和表达式的区别是什么？](https://stackoverflow.com/questions/12703214/javascript-difference-between-a-statement-and-an-expression)

<!-- Whenever possible, link a more detailed explanation. -->

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
