### React 中元素（Element）和组件（Component）的区别是什么？

#### Answer

元素是一个纯 JavaScript 对象，代表了一个 DOM 节点或者组件。元素是纯粹的、不可变的，并且创建消耗低。

一个组件是一个函数或者类（Class）。组件可以有状态，接收参数（props），并且返回一个元素树（尽管他们可以表示一个通用的容器或者包装器，并且不一定必须要生成 DOM）。组件可以在生命周期方法里面触发副作用（Side effects），比如 AJAX 请求、DOM 变动、调用第三方库，并且创建可能会很昂贵。

```js
const Component = () => "Hello"
const componentElement = <Component />
const domNodeElement = <div />
```

#### Good to hear

* 元素是不可变的纯对象，描述了你要创建的 DOM 节点或者组件。
* 组件可以是类或者函数，接收参数并且返回元素树（Element Tree）

##### Additional links

* [React docs on Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
* [React docs on Components and Props](https://reactjs.org/docs/components-and-props.html)

<!-- tags: (react,javascript) -->

<!-- expertise: (0) -->
