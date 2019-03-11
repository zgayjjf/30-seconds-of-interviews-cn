### 为什么要把整个 JavaScript 源文件包括在一个立即执行函数里面？

#### Answer

这种方式在 JavaScript 里面很常见。它创建了一个包含了整个文件内容的闭包（closure），从而创建了一个私有的命名空间，进而避免了模块、库之间潜在的命名冲突。

```js
const myLibrary = (function() {
  var privateVariable = 2
  return {
    publicMethod: () => privateVariable
  }
})()
privateVariable // ReferenceError
myLibrary.publicMethod() // 2
```

#### Good to hear

* 在很多流行的 JavaScript 库中很流行。
* 创建了一个私有命名空间。

##### Additional links

* [MDN 文档：闭包](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
