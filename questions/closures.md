### 闭包（closure）是什么？你可以给一个有用的例子嘛？

#### Answer

闭包是一个定义在其他函数里面的函数，并且有权访问其词法作用域（lexical scope）—— 甚至于当它在运行在其词法作用域以外的时候。闭包有权访问以下三个作用域的变量：

* 定义在其自身作用域的变量
* 定义在其父函数作用域的变量
* 定义在全局作用域的变量

在 JavaScript，所有的函数都是闭包，因为他们有权限访问外部的作用域，但是大部分函数没有充分利用闭包的特性：状态保存。这也是为什么闭包有时候被称为状态函数（stateful function）

另外，闭包也是 JavaScript 里面唯一的保存外部无法访问的私有数据的方式。这是 UMD（Universal Module Definition）模式的关键，经常用于库里面，可以让库只暴露公开 API，但是让其实现细节（implementation detail）保持私密，避免了和其他库或者用户的代码的命名冲突。

#### Good to hear

* 闭包非常有用，因为它允许你将数据和操作该数据的函数关联起来。
* 一个闭包可以用一个函数替代一个对象。
* 闭包可以用于模拟私有属性和方法。

##### Additional links

* [MDN docs for closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)
* [什么是闭包](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36)
* [我从未理解 JavaScript 的闭包](https://medium.com/dailyjs/i-never-understood-javascript-closures-9663703368e8)

<!-- tags: (javascript) -->

<!-- expertise: (2) -->
