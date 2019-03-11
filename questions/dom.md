### DOM 是什么？

#### Answer

DOM（文档对象模型，Document Object Model）是一个跨平台的 API，它将 HTML 和 XML 文档视为一个节点（node）组成的树形结构。这些节点（比如元素和文本节点）是可以被程序操作的对象，并且任何可见的变化都会实时反映到文档上。在一个浏览器中，JavaScript 可以用这个 API 操作 DOM 节点，改变它们的在文档中的样式、内容和位置，或者通过事件监听器与 DOM 交互。

#### Good to hear

* DOM 被设计为独立于任何特定的编程语言，使得文档的结构可以从一个一致的 API 中获得。
* 在页面加载时，DOM 被逐渐地在浏览器中构建，这也是为什么脚本通常被放在页面的底部，或者放在 `<head>` 中并带有 `defer` 属性，或者放在一个事件监听器里面。操纵 DOM 节点的脚本应该在 DOM 构建完成之后再运行，以防止出现错误。
* `document.getElementById()` 和 `document.querySelector()` 是通常用来选择 DOM 节点的函数。
* 当一个节点的 `innerHTML` 设置为一个新值时，HTML 解析器会解析该字符串。这是一种向向节点添加动态 HTML 的简单方式。

##### Additional links

* [MDN docs for DOM](https://developer.mozilla.org/en-US/docs/DOM)

<!-- tags: (html,javascript) -->

<!-- expertise: (1) -->
