### 如何避免回调地狱？

```js
getData(function(a) {
  getMoreData(a, function(b) {
    getMoreData(b, function(c) {
      getMoreData(c, function(d) {
        getMoreData(d, function(e) {
          // ...
        })
      })
    })
  })
})
```

#### Answer

一般最好的方式是用 `async/await` 将函数重构，使其返回一个 promise。相比较于给函数传递一个回调而造成深层的嵌套，这种方式可以返回一个可以用于 `await` 的 promise，并且可以在数据一返回就被处理，而下一行代码也可以以一种类似同步（sync-like）的方式执行。

上面的代码可以被重构如下：

```js
async function asyncAwaitVersion() {
  const a = await getData()
  const b = await getMoreData(a)
  const c = await getMoreData(b)
  const d = await getMoreData(c)
  const e = await getMoreData(d)
  // ...
}
```

有很多可以解决回调地狱的方法：

* 模块化（Modularization）：将回调拆分成独立的函数。
* 使用一个流程控制库，比如 async。
* 搭配 generator 使用 promise。
* 使用 async/await （node v7 以上）。

#### Good to hear

* 作为一个高效的 JavaScript 开发者，你必须要避免不断增长的缩进级别，要书写干净且可读的代码，并且可以处理复杂的流程。

##### Additional links

* [避免 Node.js 中的回调地狱](http://stackabuse.com/avoiding-callback-hell-in-node-js/)
* [异步 JavaScript：从 Callback 到 Async、Await](https://blog.hellojs.org/asynchronous-javascript-from-callback-hell-to-async-and-await-9b9ceb63c8e8)

<!-- tags: (node,javascript) -->

<!-- expertise: (2) -->
