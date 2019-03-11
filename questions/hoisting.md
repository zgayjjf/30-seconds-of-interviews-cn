### JavaScript 中的变量提升（Hoisting）是如何工作的？

#### Answer

变量提升是 JavaScript 的一种机制，变量和函数声明会在编译阶段被放到内存中去。这意味着，无论函数和变量在哪里被声明，也无论作用域是全局（global）还是局部（local），它们都会被移动到作用域的顶部，

然而，赋值是不会随着声明提升的。

以下代码段：

```js
console.log(hoist)
var hoist = "value"
```

和以下代码段等价：

```js
var hoist
console.log(hoist)
hoist = "value"
```

所以打印变量 `hoist` 会输出 `undefined` 而不是 `"value"`。

变量提升也允许你在一个函数声明（Function declaration）的位置之前调用一个函数。

```js
myFunction() // 没有错误; 打印 "hello"
function myFunction() {
  console.log("hello")
}
```

但是小心函数表达式（Function expression）有所不同：

```js
myFunction() // Error: `myFunction` is not a function
var myFunction = function() {
  console.log("hello")
}
```

#### Good to hear

* 变量提升是 JavaScript 的默认行为，其将变量提升到作用域顶部。
* 函数声明会被提升到变量声明之前。

##### Additional links

* [MDN docs for hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)
* [理解 JavaScript 中的变量提升](https://scotch.io/tutorials/understanding-hoisting-in-javascript)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
