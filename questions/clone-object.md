### 如何在 JavaScript 中复制一个对象？

#### Answer

使用对象扩展运算符（Object spread operator） `...`，对象自身的可枚举属性就会被复制到新的对象中。这可以创建一个对象的浅拷贝（Shallow clone）。

```js
const obj = { a: 1, b: 2 }
const shallowClone = { ...obj }
```

这种方法忽略掉了原型（prototype）。此外，嵌套的对象没有被复制，而是复制了他们的引用（reference），所以嵌套的对象会仍然引用与原始对象相同的对象。为了更高效地复制对象里可能嵌套的任何类型的对象（Date、RegExp、Function、Set等），深拷贝（Deep-cloning）更为复杂。

其他方法包括：

* `JSON.parse(JSON.stringify(obj))` 可以用于深拷贝一个简单的对象，但是是非常消耗 CPU 的，并且只接受有效的 JSON（因此他会跳过函数，并且不允许循环引用）
* `Object.assign({}, obj)` 是另一种方法。
* `Object.keys(obj).reduce((acc, key) => (acc[key] = obj[key[, acc), {})` 是另一个更详尽的替代方案，它更深入地展示了这个概念。

#### Good to hear

* JavaScript 通过引用传递对象，意味着说嵌套的对象的引用会被复制，而不是他们的值。
* 合并两个对象也可以用同样的方法。

##### Additional links

<!-- Whenever possible, link a more detailed explanation. -->

* [MDN docs for Object.assign()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
* [用纯 JS 复制一个对象](http://voidcanvas.com/clone-an-object-in-vanilla-js-in-depth/)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
