### Key 是什么？在列表里面使用它有什么好处？

#### Answer

Key 是一种特殊的字符串属性，帮助 React 识别哪个元素改变、增加或者移除了。它们用于渲染数组时给它们一个稳定的标识。每一个元素的 key 都应该是独一无二的（比如数据中的 ID，或者最起码需要是序号）。

```js
const todoItems = todos.map(todo => <li key={todo.id}>{todo.text}</li>)
```

* 如果内容的顺序会改变，那么不推荐使用序号（Index）作为 key，因为这会降低性能并且引发组件的状态问题。
* 如果你把列表项提取出来作为一个组件，那么要把 key 使用在列表组件上，而不是 `<li>` 标签上。

#### Good to hear

* key 一个元素在集合中的稳定标识，并帮助 React 识别变化。
* 如果元素的顺序可能变化，那应该避免使用序号作为 key。
* 如果你把列表项提取出来成为组件，你应该将 key 应用在组件上，而不是 `<li>` 元素上。

##### Additional links

* [React 文档：列表和 Key](https://reactjs.org/docs/lists-and-keys.html)

<!-- tags: (react,javascript) -->

<!-- expertise: (1) -->
