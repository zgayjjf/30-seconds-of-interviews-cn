### 无状态组件是什么？

#### Answer

无状态组件的行为不依赖于自身的状态。无状态组件可以是函数组件或者类组件。无状态函数组件更方便维护和测试，因为他们会保证在相同的参数下生成相同的输出。在没有用到生命周期钩子（Hooks）的情况下，应该优先使用无状态函数组件。

#### Good to hear

* 无状态组件独立于他们的状态。
* 无状态组件可以是类组件或函数式组件。
* 无状态函数组件应该完全避免使用 `this` 关键词。

##### Additional links

* [React 文档 - 状态和生命周期](https://reactjs.org/docs/state-and-lifecycle.html)

<!-- tags: (react,javascript) -->

<!-- expertise: (0) -->
