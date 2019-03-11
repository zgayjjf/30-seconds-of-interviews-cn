### 事件代理是什么，为什么用它？你能举一个使用它的例子嘛？

#### Answer

事件代理是一种方法，将事件代理到一个公共的祖先上。由于事件冒泡（Event bubbling），事件会顺着 DOM 树向上冒泡，并且逐步地调用每一个在监听该事件的祖先节点上的处理函数，直到根节点。

DOM 事件对象通过 `Event.target` 提供了事件触发元素的信息。这允许父元素进行响应，就好像目标元素在监听该事件一样，而不是父元素或者父元素的子元素。

这带来了两个主要好处：

* 由于只注册了了一个事件处理函数来处理可能存在的上千个元素，这可以提高性能并且降低内存占用。
* 如果元素被动态地添加到了父元素里面，不用为它们注册新的时间监听器。

相比于以下：

```js
document.querySelectorAll("button").forEach(button => {
  button.addEventListener("click", handleButtonClick)
})
```

事件代理需要用一个条件来保证子元素和目标元素相匹配：

```js
document.addEventListener("click", e => {
  if (e.target.closest("button")) {
    handleButtonClick()
  }
})
```

#### Good to hear

* 事件冒泡和捕获（capturing）的区别是什么？

##### Additional links

<!-- Whenever possible, link a more detailed explanation. -->

* [Event Delegation](https://davidwalsh.name/event-delegate)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
