### HTML 和 React 的事件处理有什么区别？

#### Answer

在 HTML 里面，参数名全部是小写的，通过提供一个字符串用来调用一个已经定义好的函数：

```html
<button onclick="handleClick()"></button>
```

在 React 中，参数名是驼峰的（camelCase），而且是在花括号里面传入一个函数引用。

```js
<button onClick={handleClick} />
```

在 HTML 里面，可以返回 `false` 来阻止默认行为，而 React 中必须明确地调用 `preventDefault`。

```html
<a href="#" onclick="console.log('The link was clicked.'); return false" />
```

```js
function handleClick(e) {
  e.preventDefault()
  console.log("The link was clicked.")
}
```

#### Good to hear

* HTML 使用小写，React 使用驼峰。

##### Additional links

* [React 文档：事件处理](https://reactjs.org/docs/handling-events.html)

<!-- tags: (react,javascript,html) -->

<!-- expertise: (1) -->
