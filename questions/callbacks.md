### 什么是回调（Callback）？你可以举一个使用回调的例子吗？

#### Answer

回调是作为参数传入其他函数的函数，并在一个事件发生或者特定的任务完成之后被调用，经常用于异步的代码。回调函数在之后被一段代码调用，但是可以在初始化阶段就声明而不必被调用。

例如，时间监听器作为异步的回调，只会在特定的事件发生时执行。

```js
function onClick() {
  console.log("用户点击了页面")
}
document.addEventListener("click", onClick)
```

然而，回调也可以是同步的。下面的 `map` 函数接受一个回调函数参数，该函数在循环的每次迭代（数组元素）中同步调用。

```js
const map = (arr, callback) => {
  const result = []
  for (let i = 0; i < arr.length; i++) {
    result.push(callback(arr[i], i))
  }
  return result
}
map([1, 2, 3, 4, 5], n => n * 2) // [2, 4, 6, 8, 10]
```

#### Good to hear

* 函数在 JavaScript 中是一等公民（First-class objects）
* 回调 vs Promise

##### Additional links

<!-- Whenever possible, link a more detailed explanation. -->

* [MDN docs for callbacks](https://developer.mozilla.org/en-US/docs/Glossary/Callback_function)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
