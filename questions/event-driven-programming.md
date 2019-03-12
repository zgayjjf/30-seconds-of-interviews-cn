### 什么是事件驱动编程？

#### Answer

时间驱动编程是一种范式，它涉及到构建一个发送和接收事件的应用。当程序发送事件的时候，程序会通过执行所有注册在这个事件上的回调函数，并将相关数据传入该函数。使用这种模式，即便没有函数订阅该事件，也可以将事件释放到外部而不引发错误。

一个通常的例子是，元素监听 DOM 事件，比如 `click` 和 `mouseenter`，当事件发生时，回调函数会被运行。

```js
document.addEventListener("click", function(event) {
  // This callback function is run when the user
  // clicks on the document.
})
```

在没有 DOM 上下文（context）的情况下，该模式可能是这样的：

```js
const hub = createEventHub()
hub.on("message", function(data) {
  console.log(`${data.username} said ${data.text}`)
})
hub.emit("message", {
  username: "John",
  text: "Hello?"
})
```

在这种实现中，`on` 是*订阅*一个事件的方法，`emit` 是*发布*一个事件的方法。

#### Good to hear

* 遵循发布-订阅（publish-subscribe）模式。
* 通过执行所有订阅该事件的回调函数来响应该事件。
* 展示如何用 JavaScript 创建一个简单的发布-订阅模式。

##### Additional links

* [MDN 文档：事件和处理器](https://developer.mozilla.org/en-US/docs/Web/Guide/Events/Overview_of_Events_and_Handlers)
* [理解 Node.js 的事件驱动（event-driven）架构](https://medium.freecodecamp.org/understanding-node-js-event-driven-architecture-223292fcbc2d)

<!-- tags: (javascript) -->

<!-- expertise: (2) -->
