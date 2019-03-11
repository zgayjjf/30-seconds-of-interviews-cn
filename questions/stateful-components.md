### React 中的有状态组件（Stateful Component）是什么意思？

#### Answer

有状态组件是其行为依赖于状态的组件。这意味着，如果给一个组件的两个不同的实例以相同的参数，不一定会渲染出相同的结果，这一点不同于纯函数组件（Pure Function Component）。

```js
// 有状态类组件（Stateful class component）
class App extends Component {
  constructor(props) {
    super(props)
    this.state = { count: 0 }
  }
  render() {
    // ...
  }
}

// 无状态组件（Stateful function component）
function App() {
  const [count, setCount] = useState(0)
  return // ...
}
```

#### Good to hear

* 有状态组件具有它们依赖的内部状态。
* 有状态组件包括类组件和使用了有状态 Hooks 的函数组件。
* 有状态组件在他们的构造函数（constructor）里面或者用 `useState()` 来初始化状态。

##### Additional links

* [React 文档 - 状态和生命周期](https://reactjs.org/docs/state-and-lifecycle.html)

<!-- tags: (react,javascript) -->

<!-- expertise: (0) -->
