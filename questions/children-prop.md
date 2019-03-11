### `children` 参数是什么？

#### Answer

`children` 是传递给组件的参数对象的一部分，它允许组件可以像数据一样被传递给其他组件，这提供了一种更干净的组合（compose）的方式。React API 中有很多方法可以用于这个参数，比如 `React.Children.map`、`React.Children.forEach`、`React.Children.only`、`React.Childnren.toArray`. 一个简单的子元素参数的例子如下：

```js
function GenericBox({ children }) {
  return <div className="container">{children}</div>
}

function App() {
  return (
    <GenericBox>
      <span>Hello</span> <span>World</span>
    </GenericBox>
  )
}
```

#### Good to hear

* 子元素（Children）是一个允许组件像数据一样被传递给其他组件的参数。
* React API 提供了使用这个属性的方法。

##### Additional links

* [React docs on Children](https://reactjs.org/docs/jsx-in-depth.html#children-in-jsx)

<!-- tags: (react,javascript) -->

<!-- expertise: (2) -->
