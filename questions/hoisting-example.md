### 这个例子中，控制台会输出什么？

```js
var foo = 1
var foobar = function() {
  console.log(foo)
  var foo = 2
}
foobar()
```

#### Answer

由于变量提升（Hoisting），局部变量会 `foo` 会在 `console.log` 调用之前声明。这意味着局部变量而不是全局变量的 `foo` 会作为一个参数被传入 `console.log`。然而，由于只有变量声明被提升，其值没有提升，所以输出会是 `undefined`，而不是 `2`。

#### Good to hear

* 变量提升是 JavaScript 的默认行为，会将声明移动到顶部。
* 提到严格（`strict`）模式。

##### Additional links

* [MDN 文档：提升](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
