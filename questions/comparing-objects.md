### 如何在 JavaScript 中对比两个对象？

#### Answer

在使用 `==` 和 `===` 时，两个不同的对象尽管可能拥有同样的属性和相同的值，他们也不会被认为是相等的。这是因为他们是通过引用（内存中的位置）比较的，不像原始类型是通过值来比较的。

我们需要一个帮助函数，来检查两个对象是否在结构上是相同的。它会遍历每个对象自身所有的属性，检查它们是不是拥有同样的值——包括嵌套的对象。
另外，还可以通过传递第三个参数 `true` 来检查它们的原型是否等价。

Note: this technique does not attempt to test equivalence of data structures other than
plain objects, arrays, functions, dates and primitive values.
注意：这个方法不会尝试检查除了普通对象（Plain Object）、数组、函数、日期和原始值以外的其他数据结构的等价性。

```js
function isDeepEqual(obj1, obj2, testPrototypes = false) {
  if (obj1 === obj2) {
    return true
  }

  if (typeof obj1 === "function" && typeof obj2 === "function") {
    return obj1.toString() === obj2.toString()
  }

  if (obj1 instanceof Date && obj2 instanceof Date) {
    return obj1.getTime() === obj2.getTime()
  }

  if (
    Object.prototype.toString.call(obj1) !==
      Object.prototype.toString.call(obj2) ||
    typeof obj1 !== "object"
  ) {
    return false
  }

  const prototypesAreEqual = testPrototypes
    ? isDeepEqual(
        Object.getPrototypeOf(obj1),
        Object.getPrototypeOf(obj2),
        true
      )
    : true

  const obj1Props = Object.getOwnPropertyNames(obj1)
  const obj2Props = Object.getOwnPropertyNames(obj2)

  return (
    obj1Props.length === obj2Props.length &&
    prototypesAreEqual &&
    obj1Props.every(prop => isDeepEqual(obj1[prop], obj2[prop]))
  )
}
```

#### Good to hear

* 字符串和数字这样的原始数据类型，是通过它们的值来比较的。
* 对象则是通过它们的引用（内存中的位置）来比较的。

##### Additional links

* [JavaScript 中的对象相等](http://adripofjavascript.com/blog/drips/object-equality-in-javascript.html)
* [两个值的深度比较](https://30secondsofcode.org/object#equals)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
