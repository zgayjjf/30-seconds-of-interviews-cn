### CORS 是什么？

#### Answer

跨域资源共享（Cross-Origin Resource Sharing）是一个使用附加的 HTTP 头来给浏览器授予权限的机制，以使其可以访问不同于当前网站源（Origin）的服务器的资源。

举跨域请求的一个例子：一个 `http://mydomain.com` 下的应用发出了一个到 `http://yourdomain.com` 的 AJAX 请求。

为了安全原因，浏览器限制了 JavaScript 发起的跨域 HTTP 请求。`XMLHttpRequest` 和 `fetch` 都遵循同源策略，意味着一个 Web 应用用这些 API 只能请求同源的 HTTP 资源，除非其他源的响应里面包含了正确的 CORS 响应头。

#### Good to hear

* CORS 行为不是错误，而是一种保护用户的机制。
* CORS 被设计用来保护用户，以防用户无意间访问了一个恶意的网站，而该网站请求了正常网站的数据从而读取用户的数据或者执行违背用户意愿的行为。

##### Additional links

<!-- Whenever possible, link a more detailed explanation. -->

* [MDN docs for CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
