### 什么是上下文（Context）？

#### Answer

上下文提供了一种通过组件树传递数据的方式，而不需要手动地在每层把参数传递下去。比如，授权的用户、语言信息、UI 主题这些需要被应用中的很多组件获取的数据。

```js
const { Provider, Consumer } = React.createContext(defaultValue)
```

#### Good to hear

* 上下文提供了一个在 React 组件树中传递数据的方式，而不需要手动地传递参数。
* 上下文被设计用来在 React 组件树中共享可以被视为*全局*的数据。

##### Additional links

* [React 文档：上下文](https://reactjs.org/docs/context.html)

<!-- tags: (react,javascript) -->

<!-- expertise: (2) -->
