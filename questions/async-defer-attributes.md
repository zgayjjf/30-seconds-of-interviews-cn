### `<script>` 标签里面的 `defer` 和 `async` 属性是什么？

#### Answer

如果两个属性都没写，脚本（script）会被串行地下载并执行，并且会暂停对文档（document）的解析（parsing），直到脚本执行完毕（默认行为）。脚本会按照其出现的顺序来下载并执行。

`defer` 属性在文档解析的同时下载脚本，但是会在文档解析完成之后再执行它，相当于在 `DOMContentLoaded` 事件监听器中执行脚本。所有 `defer` 的脚本会顺序执行。

`async` 属性会在文档解析的同时下载脚本，但是如果在文档解析完之前完成脚本下载，会前暂停文档解析，转而去执行脚本。`async` 的脚本执行不一定按照熟顺序。

注意：两个属性都应该用于带有 `src` 标签的 script 上（比如，非内联脚本）

```html
<script src="myscript.js"></script>
<script src="myscript.js" defer></script>
<script src="myscript.js" async></script>
```

#### Good to hear

* 在 `<head>` 里面放 `defer` 脚本，可以让浏览器在页面解析的同时下载脚本，因此相比于把脚本放在 body 末尾，这是一个更好的选择。
* 如果脚本之间有依赖，使用 `defer`。
* 如果脚本是独立的，使用 `async`。
* 如果 DOM 必须已经准备好并且脚本内容没有放在 `DOMContentLoaded` 监听器里面，使用 `defer`。

##### Additional links

<!-- Whenever possible, link a more detailed explanation. -->

* [async vs defer attributes](http://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html)

<!-- tags: (html) -->

<!-- expertise: (1) -->
