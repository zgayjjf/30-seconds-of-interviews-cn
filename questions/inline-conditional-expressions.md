### 什么是内联条件表达式（Inline condition expression）？

#### Answer

由于 JSX 元素树是一个大的表达式，你无法在其中嵌入语句（Statement）。在树里面，条件表达式可以用于替代语句。

例如，下面代码不会运行：

<!-- prettier-ignore -->
```js
function App({ messages, isVisible }) {
  return (
    <div>
      if (messages.length > 0) {
        <h2>You have {messages.length} unread messages.</h2>
      } else {
        <h2>You have no unread messages.</h2>
      }
      if (isVisible) {
        <p>I am visible.</p>
      }
    </div>
  )
}
```

逻辑与 `&&` 和 三元操作符 `? :` 可以替代 `if`/`else`语句。

```js
function App({ messages, isVisible }) {
  return (
    <div>
      {messages.length > 0 ? (
        <h2>You have {messages.length} unread messages.</h2>
      ) : (
        <h2>You have no unread messages.</h2>
      )}
      {isVisible && <p>I am visible.</p>}
    </div>
  )
}
```

#### Good to hear

##### Additional links

* [React 文档：条件渲染](https://reactjs.org/docs/conditional-rendering.html)

<!-- tags: (react,javascript) -->

<!-- expertise: (1) -->
