### Promise 可以处于哪些状态？

#### Answer

`Promise` 可以处于这些状态：

* pending: 初始状态，没有 fulfilled，也没有 rejected。
* fulfilled: 意味着操作已经成功完成。
* rejected: 意味着操作失败。

一个 pending 的 promise，可以被通过一个值（value）转化为 fulfilled 状态, 或者用一个原因（Error 错误）变为 rejected 状态当以上任何一个发生的时候，promise 的 then 方法注册的函数，会按照其调用顺序排队执行。

#### Good to hear

##### Additional links

* [Official Web Docs - Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

<!-- tags: (javascript) -->

<!-- expertise: (0) -->
