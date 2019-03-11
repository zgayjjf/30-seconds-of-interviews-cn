### 回调引用（callback refs） 和 findDOMNode()，哪个更好？

#### Answer

回调引用优于 `findDOMNode())` API，这是因为 `findDOMNode()` 影响了 React 未来的一些改进。

```js
// 之前使用 `findDOMNode()` 的方式。
class MyComponent extends Component {
  componentDidMount() {
    findDOMNode(this).scrollIntoView()
  }

  render() {
    return <div />
  }
}

// 推荐使用回调引用的方式。
class MyComponent extends Component {
  componentDidMount() {
    this.node.scrollIntoView()
  }

  render() {
    return <div ref={node => (this.node = node)} />
  }
}
```

#### Good to hear

* 更推荐使用回调引用而不是 `findDOMNode()`。

##### Additional links

* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html#exposing-dom-refs-to-parent-components)

<!-- tags: (react,javascript) -->

<!-- expertise: (2) -->
