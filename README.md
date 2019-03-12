<h1 align="center">
  30 秒前端面试题
</h1>

<h4 align="center">精选常见前端面试题集，帮助你为下一次面试做准备。</h4>

<br>

<p align="center">
  <a href="https://gitter.im/30-seconds-of-interviews/Lobby"><img src="https://img.shields.io/badge/gitter-join%20chat%20%E2%86%92-brightgreen.svg" alt="gitter"></a>
    <a href="https://github.com/fejes713/30-seconds-of-interviews/blob/master/CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs welcome"></a>
  <a href="https://travis-ci.com/30-seconds/30-seconds-of-interviews"><img src="https://travis-ci.com/30-seconds/30-seconds-of-interviews.svg?token=uZrzJhwCxqfwx7TdXzc4&branch=master" alt="travis"></a>
  <a href="https://www.producthunt.com/posts/30-seconds-of-interviews"><img src="https://img.shields.io/badge/Product%20Hunt-vote-orange.svg" alt="producthunt"></a>
  <a href="https://github.com/30-seconds/30-seconds-of-interviews/blob/master/LICENSE"><img src="https://img.shields.io/badge/licence-MIT-blue.svg" alt="licence"></a>
</p>

<br>

> *该 README 使用 [markdown-builder](https://github.com/30-seconds/markdown-builder) 构建.*

## 前言

面试是很可怕的，甚至可以让最有经验的专家在压力之下忘记如何回答。一起来了解这些社区收集的面试中常见问题，为面试官提出的任何问题做好准备。通过把经验总结和现实例子结合起来，可以让你从紧张到从容不迫地迎接下一个机会。

## [在线查看（英文）](https://30secondsofinterviews.org/)

## 贡献

> 30 秒前端面试题是一个社区的成果，所以请尽你所能贡献自己的力量。每一个贡献都是有帮助的！

如果想加入翻译小组或者进群交流&招聘，请加微信入群：simple_robot。

![simple_robot](./wechat-simple_robot.png)


如果想提交面试题，请阅读 [贡献指南](https://github.com/30-seconds/30-seconds-of-interviews/blob/master/CONTRIBUTING.md) 并在原仓库提交一个 pull request。

#### 相关项目

- [30 Seconds of Code](https://30secondsofcode.org)
- [30 Seconds of CSS](https://30-seconds.github.io/30-seconds-of-css/)
- [30 Seconds of React](https://github.com/30-seconds/30-seconds-of-react)
- [30 Seconds of Knowledge](https://chrome.google.com/webstore/detail/30-seconds-of-knowledge/mmgplondnjekobonklacmemikcnhklla)

## 内容


### JavaScript

<details>
<summary>查看详情</summary>

* [创建一个 `batches` 函数，返回根据一个食谱可以烹饪的食物的最大数量。](#创建一个-batches-函数，返回根据一个食谱可以烹饪的食物的最大数量。)
* [什么是大 O 符号？](#什么是大-o-符号？)
* [创建一个独立的 `bind` 函数，其功能等价于 `Function.prototype.bind` 。](#创建一个独立的-bind-函数，其功能等价于-functionprototypebind-。)
* [如何避免回调地狱？](#如何避免回调地狱？)
* [`setState` 的回调函数（Callback function）参数有什么用？](#setstate-的回调函数（callback-function）参数有什么用？)
* [回调引用（callback refs） 和 findDOMNode()，哪个更好？](#回调引用（callback-refs）-和-finddomnode，哪个更好？)
* [什么是回调（Callback）？你可以举一个使用回调的例子吗？](#什么是回调（callback）？你可以举一个使用回调的例子吗？)
* [`children` 参数是什么？](#children-参数是什么？)
* [如何在 JavaScript 中复制一个对象？](#如何在-javascript-中复制一个对象？)
* [闭包（closure）是什么？你可以给一个有用的例子嘛？](#闭包（closure）是什么？你可以给一个有用的例子嘛？)
* [如何在 JavaScript 中对比两个对象？](#如何在-javascript-中对比两个对象？)
* [什么是上下文（Context）？](#什么是上下文（context）？)
* [CORS 是什么？](#cors-是什么？)
* [DOM 是什么？](#dom-是什么？)
* [相等操作符 `==` 和 `===` 的区别是什么？](#相等操作符--和--的区别是什么？)
* [React 中元素（Element）和组件（Component）的区别是什么？](#react-中元素（element）和组件（component）的区别是什么？)
* [事件代理是什么，为什么用它？你能举一个使用它的例子嘛？](#事件代理是什么，为什么用它？你能举一个使用它的例子嘛？)
* [什么是事件驱动编程？](#什么是事件驱动编程？)
* [JavaScript 里面表达式（Expression）和语句（Statement）的区别是什么？](#javascript-里面表达式（expression）和语句（statement）的区别是什么？)
* [JavaScript 中的真值（Truthy）和假值（Falsy）是什么？](#javascript-中的真值（truthy）和假值（falsy）是什么？)
* [生成一个包含 n 项斐波那契数列的数组。](#生成一个包含-n-项斐波那契数列的数组。)
* [`0.1 + 0.2 === 0.3` 的值是什么？](#01--02--03-的值是什么？)
* [数组方法 `map()` 和 `forEach()` 的区别是什么？](#数组方法-map-和-foreach-的区别是什么？)
* [What are fragments?](#what-are-fragments)
* [What is functional programming?](#what-is-functional-programming)
* [这个例子中，控制台会输出什么？](#这个例子中，控制台会输出什么？)
* [JavaScript 中的变量提升（Hoisting）是如何工作的？](#javascript-中的变量提升（hoisting）是如何工作的？)
* [HTML 和 React 的事件处理有什么区别？](#html-和-react-的事件处理有什么区别？)
* [为什么要把整个 JavaScript 源文件包括在一个立即执行函数里面？](#为什么要把整个-javascript-源文件包括在一个立即执行函数里面？)
* [Explain the differences between imperative and declarative programming.](#explain-the-differences-between-imperative-and-declarative-programming)
* [什么是内联条件表达式（Inline condition expression）？](#什么是内联条件表达式（inline-condition-expression）？)
* [Key 是什么？在列表里面使用它有什么好处？](#key-是什么？在列表里面使用它有什么好处？)
* [What is the difference between lexical scoping and dynamic scoping?](#what-is-the-difference-between-lexical-scoping-and-dynamic-scoping)
* [Create a function that masks a string of characters with `#` except for the last four (4) characters.](#create-a-function-that-masks-a-string-of-characters-with--except-for-the-last-four-4-characters)
* [What is memoization?](#what-is-memoization)
* [How do you ensure methods have the correct `this` context in React component classes?](#how-do-you-ensure-methods-have-the-correct-this-context-in-react-component-classes)
* [What is a MIME type and what is it used for?](#what-is-a-mime-type-and-what-is-it-used-for)
* [Contrast mutable and immutable values, and mutating vs non-mutating methods.](#contrast-mutable-and-immutable-values-and-mutating-vs-non-mutating-methods)
* [What is the only value not equal to itself in JavaScript?](#what-is-the-only-value-not-equal-to-itself-in-javascript)
* [NodeJS often uses a callback pattern where if an error is encountered during execution, this error is passed as the first argument to the callback. What are the advantages of this pattern?](#nodejs-often-uses-a-callback-pattern-where-if-an-error-is-encountered-during-execution-this-error-is-passed-as-the-first-argument-to-the-callback-what-are-the-advantages-of-this-pattern)
* [What is the event loop in Node.js?](#what-is-the-event-loop-in-nodejs)
* [What is the difference between `null` and `undefined`?](#what-is-the-difference-between-null-and-undefined)
* [Describe the different ways to create an object. When should certain ways be preferred over others?](#describe-the-different-ways-to-create-an-object-when-should-certain-ways-be-preferred-over-others)
* [What is the difference between a parameter and an argument?](#what-is-the-difference-between-a-parameter-and-an-argument)
* [Does JavaScript pass by value or by reference?](#does-javascript-pass-by-value-or-by-reference)
* [How do you pass an argument to an event handler or callback?](#how-do-you-pass-an-argument-to-an-event-handler-or-callback)
* [Create a function `pipe` that performs left-to-right function composition by returning a function that accepts one argument.](#create-a-function-pipe-that-performs-left-to-right-function-composition-by-returning-a-function-that-accepts-one-argument)
* [What are portals in React?](#what-are-portals-in-react)
* [后缀自增运算符 `i++` 和 前缀自增运算符 `++i` 有什么区别？](#后缀自增运算符-i-和-前缀自增运算符-i-有什么区别？)
* [Promise 可以处于哪些状态？](#promise-可以处于哪些状态？)
* [What are Promises?](#what-are-promises)
* [How does prototypal inheritance differ from classical inheritance?](#how-does-prototypal-inheritance-differ-from-classical-inheritance)
* [What is a pure function?](#what-is-a-pure-function)
* [What is recursion and when is it useful?](#what-is-recursion-and-when-is-it-useful)
* [What is the output of the following code?](#what-is-the-output-of-the-following-code)
* [What are refs in React? When should they be used?](#what-are-refs-in-react-when-should-they-be-used)
* [What does the following function return?](#what-does-the-following-function-return)
* [Are semicolons required in JavaScript?](#are-semicolons-required-in-javascript)
* [What is short-circuit evaluation in JavaScript?](#what-is-short-circuit-evaluation-in-javascript)
* [React 中的有状态组件（Stateful Component）是什么意思？](#react-中的有状态组件（stateful-component）是什么意思？)
* [无状态组件是什么？](#无状态组件是什么？)
* [Explain the difference between a static method and an instance method.](#explain-the-difference-between-a-static-method-and-an-instance-method)
* [What is the difference between synchronous and asynchronous code in JavaScript?](#what-is-the-difference-between-synchronous-and-asynchronous-code-in-javascript)
* [What is the `this` keyword and how does it work?](#what-is-the-this-keyword-and-how-does-it-work)
* [What does the following code evaluate to?](#what-does-the-following-code-evaluate-to)
* [What are JavaScript data types?](#what-are-javascript-data-types)
* [What is the purpose of JavaScript UI libraries/frameworks like React, Vue, Angular, Hyperapp, etc?](#what-is-the-purpose-of-javascript-ui-librariesframeworks-like-react-vue-angular-hyperapp-etc)
* [What does `'use strict'` do and what are some of the key benefits to using it?](#what-does-use-strict-do-and-what-are-some-of-the-key-benefits-to-using-it)
* [What are the differences between `var`, `let`, `const` and no keyword statements?](#what-are-the-differences-between-var-let-const-and-no-keyword-statements)
* [What is a virtual DOM and why is it used in libraries/frameworks?](#what-is-a-virtual-dom-and-why-is-it-used-in-librariesframeworks)
* [What is a cross-site scripting attack (XSS) and how do you prevent it?](#what-is-a-cross-site-scripting-attack-xss-and-how-do-you-prevent-it)
</details>


### React

<details>
<summary>查看详情</summary>

* [`setState` 的回调函数（Callback function）参数有什么用？](#setstate-的回调函数（callback-function）参数有什么用？)
* [回调引用（callback refs） 和 findDOMNode()，哪个更好？](#回调引用（callback-refs）-和-finddomnode，哪个更好？)
* [`children` 参数是什么？](#children-参数是什么？)
* [Why does React use `className` instead of `class` like in HTML?](#why-does-react-use-classname-instead-of-class-like-in-html)
* [什么是上下文（Context）？](#什么是上下文（context）？)
* [React 中元素（Element）和组件（Component）的区别是什么？](#react-中元素（element）和组件（component）的区别是什么？)
* [What are error boundaries in React?](#what-are-error-boundaries-in-react)
* [What are fragments?](#what-are-fragments)
* [What are higher-order components?](#what-are-higher-order-components)
* [HTML 和 React 的事件处理有什么区别？](#html-和-react-的事件处理有什么区别？)
* [什么是内联条件表达式（Inline condition expression）？](#什么是内联条件表达式（inline-condition-expression）？)
* [Key 是什么？在列表里面使用它有什么好处？](#key-是什么？在列表里面使用它有什么好处？)
* [What are the lifecycle methods in React?](#what-are-the-lifecycle-methods-in-react)
* [What are the different phases of the component lifecycle in React?](#what-are-the-different-phases-of-the-component-lifecycle-in-react)
* [What does lifting state up in React mean?](#what-does-lifting-state-up-in-react-mean)
* [How do you ensure methods have the correct `this` context in React component classes?](#how-do-you-ensure-methods-have-the-correct-this-context-in-react-component-classes)
* [How do you pass an argument to an event handler or callback?](#how-do-you-pass-an-argument-to-an-event-handler-or-callback)
* [What are portals in React?](#what-are-portals-in-react)
* [How to apply prop validation in React?](#how-to-apply-prop-validation-in-react)
* [How do you write comments inside a JSX tree in React?](#how-do-you-write-comments-inside-a-jsx-tree-in-react)
* [What are refs in React? When should they be used?](#what-are-refs-in-react-when-should-they-be-used)
* [React 中的有状态组件（Stateful Component）是什么意思？](#react-中的有状态组件（stateful-component）是什么意思？)
* [无状态组件是什么？](#无状态组件是什么？)
</details>


### HTML

<details>
<summary>查看详情</summary>

* [`image` 标签里面的 `alt` 属性有什么用？](#image-标签里面的-alt-属性有什么用？)
* [`<script>` 标签里面的 `defer` 和 `async` 属性是什么？](#script-标签里面的-defer-和-async-属性是什么？)
* [What is the purpose of cache busting and how can you achieve it?](#what-is-the-purpose-of-cache-busting-and-how-can-you-achieve-it)
* [DOM 是什么？](#dom-是什么？)
* [Can a web page contain multiple `<header>` elements? What about `<footer>` elements?](#can-a-web-page-contain-multiple-header-elements-what-about-footer-elements)
* [Discuss the differences between an HTML specification and a browser’s implementation thereof.](#discuss-the-differences-between-an-html-specification-and-a-browsers-implementation-thereof)
* [HTML 和 React 的事件处理有什么区别？](#html-和-react-的事件处理有什么区别？)
* [What are some differences that XHTML has compared to HTML?](#what-are-some-differences-that-xhtml-has-compared-to-html)
* [Briefly describe the correct usage of the following HTML5 semantic elements: `<header>`, `<article>`,`<section>`, `<footer>`](#briefly-describe-the-correct-usage-of-the-following-html5-semantic-elements-header-articlesection-footer)
* [What is HTML5 Web Storage? Explain `localStorage` and `sessionStorage`.](#what-is-html5-web-storage-explain-localstorage-and-sessionstorage)
* [Where and why is the `rel="noopener"` attribute used?](#where-and-why-is-the-relnoopener-attribute-used)
</details>


### CSS

<details>
<summary>查看详情</summary>

* [什么是 CSS BEM？](#什么是-css-bem？)
* [Describe the layout of the CSS Box Model and briefly describe each component.](#describe-the-layout-of-the-css-box-model-and-briefly-describe-each-component)
* [What are the advantages of using CSS preprocessors?](#what-are-the-advantages-of-using-css-preprocessors)
* [What is the difference between '+' and '~' sibling selectors?.](#what-is-the-difference-between--and--sibling-selectors)
* [Can you describe how CSS specificity works?](#can-you-describe-how-css-specificity-works)
* [What is the difference between `em` and `rem` units?](#what-is-the-difference-between-em-and-rem-units)
* [Using flexbox, create a 3-column layout where each column takes up a `col-{n} / 12` ratio of the container.](#using-flexbox-create-a-3-column-layout-where-each-column-takes-up-a-col-n--12-ratio-of-the-container)
* [What is a focus ring? What is the correct solution to handle them?](#what-is-a-focus-ring-what-is-the-correct-solution-to-handle-them)
* [Can you name the four types of `@media` properties?](#can-you-name-the-four-types-of-media-properties)
* [What are the advantages of using CSS sprites and how are they utilized?](#what-are-the-advantages-of-using-css-sprites-and-how-are-they-utilized)
</details>


### Node

<details>
<summary>查看详情</summary>

* [如何避免回调地狱？](#如何避免回调地狱？)
* [NodeJS often uses a callback pattern where if an error is encountered during execution, this error is passed as the first argument to the callback. What are the advantages of this pattern?](#nodejs-often-uses-a-callback-pattern-where-if-an-error-is-encountered-during-execution-this-error-is-passed-as-the-first-argument-to-the-callback-what-are-the-advantages-of-this-pattern)
* [What is the event loop in Node.js?](#what-is-the-event-loop-in-nodejs)
* [What is REST?](#what-is-rest)
</details>


### Security

<details>
<summary>查看详情</summary>

* [What is a cross-site scripting attack (XSS) and how do you prevent it?](#what-is-a-cross-site-scripting-attack-xss-and-how-do-you-prevent-it)
</details>


---

## JavaScript
### 无状态组件是什么？

<details>
<summary>查看答案</summary>

无状态组件的行为不依赖于自身的状态。无状态组件可以是函数组件或者类组件。无状态函数组件更方便维护和测试，因为他们会保证在相同的参数下生成相同的输出。在没有用到生命周期钩子（Hooks）的情况下，应该优先使用无状态函数组件。


#### 加分回答


* 无状态组件独立于他们的状态。
* 无状态组件可以是类组件或函数式组件。
* 无状态函数组件应该完全避免使用 `this` 关键词。


##### 相关链接


* [React 文档 状态和生命周期](https://reactjs.org/docs/state-and-lifecycle.html)

</details>

<br>[⬆ 回到顶部](#内容)

### 相等操作符 `==` 和 `===` 的区别是什么？

<details>
<summary>查看答案</summary>

三等号 (`===`) 检查是否严格相等，意即：类型和值都要一样。双等号则会首先进行强制类型转换，使得等号两边对象拥有同样的类型，再进行严格的比较。


#### 加分回答


* 尽可能使用三等号来做相等比较，因为宽松相等 `==` 会有反直觉的结果。
* 强制类型转换意味着所有的值都会被转化为同样的类型。
* 提到假值 (Falsy values) 和他们的比较。


##### 相关链接


* [MDN 比较操作符](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators)

</details>

<br>[⬆ 回到顶部](#内容)

### React 中元素（Element）和组件（Component）的区别是什么？

<details>
<summary>查看答案</summary>

元素是一个纯 JavaScript 对象，代表了一个 DOM 节点或者组件。元素是纯粹的、不可变的，并且创建消耗低。

一个组件是一个函数或者类（Class）。组件可以有状态，接收参数（props），并且返回一个元素树（尽管他们可以表示一个通用的容器或者包装器，并且不一定必须要生成 DOM）。组件可以在生命周期方法里面触发副作用（Side effects），比如 AJAX 请求、DOM 变动、调用第三方库，并且创建可能会很昂贵。

```js
const Component = () => "Hello"
const componentElement = <Component />
const domNodeElement = <div />
```


#### 加分回答


* 元素是不可变的纯对象，描述了你要创建的 DOM 节点或者组件。
* 组件可以是类或者函数，接收参数并且返回元素树（Element Tree）


##### 相关链接


* [React docs on Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
* [React docs on Components and Props](https://reactjs.org/docs/components-and-props.html)

</details>

<br>[⬆ 回到顶部](#内容)

### React 中的有状态组件（Stateful Component）是什么意思？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* 有状态组件具有它们依赖的内部状态。
* 有状态组件包括类组件和使用了有状态 Hooks 的函数组件。
* 有状态组件在他们的构造函数（constructor）里面或者用 `useState()` 来初始化状态。


##### 相关链接


* [React 文档 状态和生命周期](https://reactjs.org/docs/state-and-lifecycle.html)

</details>

<br>[⬆ 回到顶部](#内容)

### Promise 可以处于哪些状态？

<details>
<summary>查看答案</summary>

`Promise` 可以处于这些状态：

* pending: 初始状态，没有 fulfilled，也没有 rejected。
* fulfilled: 意味着操作已经成功完成。
* rejected: 意味着操作失败。

一个 pending 的 promise，可以被通过一个值（value）转化为 fulfilled 状态, 或者用一个原因（Error 错误）变为 rejected 状态当以上任何一个发生的时候，promise 的 then 方法注册的函数，会按照其调用顺序排队执行。


#### 加分回答




##### 相关链接


* [Official Web Docs Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

</details>

<br>[⬆ 回到顶部](#内容)

### 后缀自增运算符 `i++` 和 前缀自增运算符 `++i` 有什么区别？

<details>
<summary>查看答案</summary>

都把变量值加 1。区别在于他们什么时候求值。

后缀自增运算符在其自增**之前**求值。

```js
let i = 0
i++ // 0
// i === 1
```

前缀自增运算符在其自增**之后**求值。

```js
let i = 0
++i // 1
// i === 1
```


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### 创建一个 `batches` 函数，返回根据一个食谱可以烹饪的食物的最大数量。

```js
/**
函数接受两个对象作为参数，第一个是食物的食谱，第二个是可用的原材料。
每个原材料的值是一个数字，代表有多少单位的材料。
`batches(recipe, available)`
*/

// 可以做 0 批
batches(
  { milk: 100, butter: 50, flour: 5 },
  { milk: 132, butter: 48, flour: 51 }
)
batches(
  { milk: 100, flour: 4, sugar: 10, butter: 5 },
  { milk: 1288, flour: 9, sugar: 95 }
)

// 可以做 1 批
batches(
  { milk: 100, butter: 50, cheese: 10 },
  { milk: 198, butter: 52, cheese: 10 }
)

// 可以做 2 批
batches(
  { milk: 2, sugar: 40, butter: 20 },
  { milk: 5, sugar: 120, butter: 500 }
)
```

<details>
<summary>查看答案</summary>

我们必须有所有的配方中可用的原材料，而且数量要大于或等于所需的材料数量。只要有一个原材料不可用或低于我们需要的，我们就无法做哪怕一批。

用 `Object.keys()` 获得原材料的数组，再用 `Array.prototype.map()` 将每一个原材料映射到可用原材料的数量与配饭所需数量的比例。如果一个配方所需的原材料不可用，该比例会被计算为 `NaN`，所以或逻辑运算符 `||` 可以用于将这种情况回退到 `0`。

用扩展运算符 `...` ，将原材料数组传入 `Math.min()` 来找到最小的比例。将最后的结果传入 `Math.floor()`，从而将结果舍尾成可做的最大数量。

```js
const batches = (recipe, available) =>
  Math.floor(
    Math.min(...Object.keys(recipe).map(k => available[k] / recipe[k] || 0))
  )
```


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### What does the following code evaluate to?

```js
typeof typeof 0
```

<details>
<summary>查看答案</summary>

It evaluates to `"string"`.

`typeof 0` evaluates to the string `"number"` and therefore `typeof "number"` evaluates to `"string"`.


#### 加分回答




##### 相关链接


* [MDN docs for typeof](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof)

</details>

<br>[⬆ 回到顶部](#内容)

### 如何在 JavaScript 中复制一个对象？

<details>
<summary>查看答案</summary>

使用对象扩展运算符（Object spread operator） `...`，对象自身的可枚举属性就会被复制到新的对象中。这可以创建一个对象的浅拷贝（Shallow clone）。

```js
const obj = { a: 1, b: 2 }
const shallowClone = { ...obj }
```

这种方法忽略掉了原型（prototype）。此外，嵌套的对象没有被复制，而是复制了他们的引用（reference），所以嵌套的对象会仍然引用与原始对象相同的对象。为了更高效地复制对象里可能嵌套的任何类型的对象（Date、RegExp、Function、Set 等），深拷贝（Deep-cloning）更为复杂。

其他方法包括：

* `JSON.parse(JSON.stringify(obj))` 可以用于深拷贝一个简单的对象，但是是非常消耗 CPU 的，并且只接受有效的 JSON（因此他会跳过函数，并且不允许循环引用）
* `Object.assign({}, obj)` 是另一种方法。
* `Object.keys(obj).reduce((acc, key) => (acc[key] = obj[key[, acc), {})` 是另一个更详尽的替代方案，它更深入地展示了这个概念。


#### 加分回答


* JavaScript 通过引用传递对象，意味着说嵌套的对象的引用会被复制，而不是他们的值。
* 合并两个对象也可以用同样的方法。


##### 相关链接


* [MDN docs for Object.assign()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
* [用纯 JS 复制一个对象](http://voidcanvas.com/clone-an-object-in-vanilla-js-in-depth/)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the difference between synchronous and asynchronous code in JavaScript?

<details>
<summary>查看答案</summary>

Synchronous means each operation must wait for the previous one to complete.

Asynchronous means an operation can occur while another operation is still being processed.

In JavaScript, all code is synchronous due to the single-threaded nature of it. However, asynchronous operations not part of the program (such as `XMLHttpRequest` or `setTimeout`) are processed outside of the main thread because they are controlled by native code (browser APIs), but callbacks part of the program will still be executed synchronously.


#### 加分回答


* JavaScript has a concurrency model based on an "event loop".
* Functions like `alert` block the main thread so that no user input is registered until the user closes it.


##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### 如何在 JavaScript 中对比两个对象？

<details>
<summary>查看答案</summary>

在使用 `==` 和 `===` 时，两个不同的对象尽管可能拥有同样的属性和相同的值，他们也不会被认为是相等的。这是因为他们是通过引用（内存中的位置）比较的，不像原始类型是通过值来比较的。

我们需要一个帮助函数，来检查两个对象是否在结构上是相同的。它会遍历每个对象自身所有的属性，检查它们是不是拥有同样的值——包括嵌套的对象。另外，还可以通过传递第三个参数 `true` 来检查它们的原型是否等价。

Note: this technique does not attempt to test equivalence of data structures other than
plain objects, arrays, functions, dates and primitive values.
注意：这个方法不会尝试检查除了普通对象（Plain Object）、数组、函数、日期和原始值以外的其他数据结构的等价性。

```js
function isDeepEqual(obj1, obj2, testPrototypes = false) {
  if (obj1 === obj2) {
    return true
  }

  if (typeof obj1 === "function" && typeof obj2 === "function") {
    return obj1.toString() === obj2.toString()
  }

  if (obj1 instanceof Date && obj2 instanceof Date) {
    return obj1.getTime() === obj2.getTime()
  }

  if (
    Object.prototype.toString.call(obj1) !==
      Object.prototype.toString.call(obj2) ||
    typeof obj1 !== "object"
  ) {
    return false
  }

  const prototypesAreEqual = testPrototypes
    ? isDeepEqual(
        Object.getPrototypeOf(obj1),
        Object.getPrototypeOf(obj2),
        true
      )
    : true

  const obj1Props = Object.getOwnPropertyNames(obj1)
  const obj2Props = Object.getOwnPropertyNames(obj2)

  return (
    obj1Props.length === obj2Props.length &&
    prototypesAreEqual &&
    obj1Props.every(prop => isDeepEqual(obj1[prop], obj2[prop]))
  )
}
```


#### 加分回答


* 字符串和数字这样的原始数据类型，是通过它们的值来比较的。
* 对象则是通过它们的引用（内存中的位置）来比较的。


##### 相关链接


* [JavaScript 中的对象相等](http://adripofjavascript.com/blog/drips/object-equality-in-javascript.html)
* [两个值的深度比较](https://30secondsofcode.org/object#equals)

</details>

<br>[⬆ 回到顶部](#内容)

### What is a cross-site scripting attack (XSS) and how do you prevent it?

<details>
<summary>查看答案</summary>

XSS refers to client-side code injection where the attacker injects malicious scripts into a legitimate website or web application. This is often achieved when the application does not validate user input and freely injects dynamic HTML content.

For example, a comment system will be at risk if it does not validate or escape user input. If the comment contains unescaped HTML, the comment can inject a `<script>` tag into the website that other users will execute against their knowledge.

* The malicious script has access to cookies which are often used to store session tokens. If an attacker can obtain a user’s session cookie, they can impersonate the user.
* The script can arbitrarily manipulate the DOM of the page the script is executing in, allowing the attacker to insert pieces of content that appear to be a real part of the website.
* The script can use AJAX to send HTTP requests with arbitrary content to arbitrary destinations.


#### 加分回答


* On the client, using `textContent` instead of `innerHTML` prevents the browser from running the string through the HTML parser which would execute scripts in it.
* On the server, escaping HTML tags will prevent the browser from parsing the user input as actual HTML and therefore won't execute the script.


##### 相关链接


* [Cross-Site Scripting Attack (XSS)](https://www.acunetix.com/websitesecurity/cross-site-scripting/)

</details>

<br>[⬆ 回到顶部](#内容)

### CORS 是什么？

<details>
<summary>查看答案</summary>

跨域资源共享（Cross-Origin Resource Sharing）是一个使用附加的 HTTP 头来给浏览器授予权限的机制，以使其可以访问不同于当前网站源（Origin）的服务器的资源。

举跨域请求的一个例子：一个 `http://mydomain.com` 下的应用发出了一个到 `http://yourdomain.com` 的 AJAX 请求。

为了安全原因，浏览器限制了 JavaScript 发起的跨域 HTTP 请求。`XMLHttpRequest` 和 `fetch` 都遵循同源策略，意味着一个 Web 应用用这些 API 只能请求同源的 HTTP 资源，除非其他源的响应里面包含了正确的 CORS 响应头。


#### 加分回答


* CORS 行为不是错误，而是一种保护用户的机制。
* CORS 被设计用来保护用户，以防用户无意间访问了一个恶意的网站，而该网站请求了正常网站的数据从而读取用户的数据或者执行违背用户意愿的行为。


##### 相关链接


* [MDN docs for CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)

</details>

<br>[⬆ 回到顶部](#内容)

### DOM 是什么？

<details>
<summary>查看答案</summary>

DOM（文档对象模型，Document Object Model）是一个跨平台的 API，它将 HTML 和 XML 文档视为一个节点（node）组成的树形结构。这些节点（比如元素和文本节点）是可以被程序操作的对象，并且任何可见的变化都会实时反映到文档上。在一个浏览器中，JavaScript 可以用这个 API 操作 DOM 节点，改变它们的在文档中的样式、内容和位置，或者通过事件监听器与 DOM 交互。


#### 加分回答


* DOM 被设计为独立于任何特定的编程语言，使得文档的结构可以从一个一致的 API 中获得。
* 在页面加载时，DOM 被逐渐地在浏览器中构建，这也是为什么脚本通常被放在页面的底部，或者放在 `<head>` 中并带有 `defer` 属性，或者放在一个事件监听器里面。操纵 DOM 节点的脚本应该在 DOM 构建完成之后再运行，以防止出现错误。
* `document.getElementById()` 和 `document.querySelector()` 是通常用来选择 DOM 节点的函数。
* 当一个节点的 `innerHTML` 设置为一个新值时，HTML 解析器会解析该字符串。这是一种向向节点添加动态 HTML 的简单方式。


##### 相关链接


* [MDN docs for DOM](https://developer.mozilla.org/en-US/docs/DOM)

</details>

<br>[⬆ 回到顶部](#内容)

### 创建一个独立的 `bind` 函数，其功能等价于 `Function.prototype.bind` 。

```js
function example() {
  console.log(this)
}
const boundExample = bind(example, { a: true })
boundExample.call({ b: true }) // logs { a: true }
```

<details>
<summary>查看答案</summary>

返回一个函数，该函数接受任意数量的参数，并将它们用剩余参数运算符 `...` 收集起来。该函数使用 `fn` 调用 `Function.prototype.apply` 并传入上下文（context）和传入的参数数组，最后将结果返回。

```js
const bind = (fn, context) => (...args) => fn.apply(context, args)
```


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### What are the differences between `var`, `let`, `const` and no keyword statements?

<details>
<summary>查看答案</summary>

##### No keyword

When no keyword exists before a variable assignment, it is either assigning a global variable if one does not exist, or reassigns an already declared variable. In non-strict mode, if the variable has not yet been declared, it will assign the variable as a property of the global object (`window` in browsers). In strict mode, it will throw an error to prevent unwanted global variables from being created.

##### var

`var` was the default statement to declare a variable until ES2015. It creates a function-scoped variable that can be reassigned and redeclared. However, due to its lack of block scoping, it can cause issues if the variable is being reused in a loop that contains an asynchronous callback because the variable will continue to exist outside of the block scope.

Below, by the time the the `setTimeout` callback executes, the loop has already finished and the `i` variable is `10`, so all ten callbacks reference the same variable available in the function scope.

```js
for (var i = 0; i < 10; i++) {
  setTimeout(() => {
    // logs `10` ten times
    console.log(i)
  })
}

/* Solutions with `var` */
for (var i = 0; i < 10; i++) {
  // Passed as an argument will use the value as-is in
  // that point in time
  setTimeout(console.log, 0, i)
}

for (var i = 0; i < 10; i++) {
  // Create a new function scope that will use the value
  // as-is in that point in time
  ;(i => {
    setTimeout(() => {
      console.log(i)
    })
  })(i)
}
```

##### let

`let` was introduced in ES2015 and is the new preferred way to declare variables that will be reassigned later. Trying to redeclare a variable again will throw an error. It is block-scoped so that using it in a loop will keep it scoped to the iteration.

```js
for (let i = 0; i < 10; i++) {
  setTimeout(() => {
    // logs 0, 1, 2, 3, ...
    console.log(i)
  })
}
```

##### const

`const` was introduced in ES2015 and is the new preferred default way to declare all variables if they won't be reassigned later, even for objects that will be mutated (as long as the reference to the object does not change). It is block-scoped and cannot be reassigned.

```js
const myObject = {}
myObject.prop = "hello!" // No error
myObject = "hello" // Error
```


#### 加分回答


* All declarations are hoisted to the top of their scope.
* However, with `let` and `const` there is a concept called the temporal dead zone (TDZ). While the declarations are still hoisted, there is a period between entering scope and being declared where they cannot be accessed.
* Show a common issue with using `var` and how `let` can solve it, as well as a solution that keeps `var`.
* `var` should be avoided whenever possible and prefer `const` as the default declaration statement for all variables unless they will be reassigned later, then use `let` if so.


##### 相关链接


* [`let` vs `const`](https://wesbos.com/let-vs-const/)

</details>

<br>[⬆ 回到顶部](#内容)

### 事件代理是什么，为什么用它？你能举一个使用它的例子嘛？

<details>
<summary>查看答案</summary>

事件代理是一种方法，将事件代理到一个公共的祖先上。由于事件冒泡（Event bubbling），事件会顺着 DOM 树向上冒泡，并且逐步地调用每一个在监听该事件的祖先节点上的处理函数，直到根节点。

DOM 事件对象通过 `Event.target` 提供了事件触发元素的信息。这允许父元素进行响应，就好像目标元素在监听该事件一样，而不是父元素或者父元素的子元素。

这带来了两个主要好处：

* 由于只注册了了一个事件处理函数来处理可能存在的上千个元素，这可以提高性能并且降低内存占用。
* 如果元素被动态地添加到了父元素里面，不用为它们注册新的时间监听器。

相比于以下：

```js
document.querySelectorAll("button").forEach(button => {
  button.addEventListener("click", handleButtonClick)
})
```

事件代理需要用一个条件来保证子元素和目标元素相匹配：

```js
document.addEventListener("click", e => {
  if (e.target.closest("button")) {
    handleButtonClick()
  }
})
```


#### 加分回答


* 事件冒泡和捕获（capturing）的区别是什么？


##### 相关链接


* [Event Delegation](https://davidwalsh.name/event-delegate)

</details>

<br>[⬆ 回到顶部](#内容)

### `setState` 的回调函数（Callback function）参数有什么用？

<details>
<summary>查看答案</summary>

回调函数在 `setState` 执行完毕，并且组件渲染完毕之后调用。由于 `setState` 是异步的，回调函数可以用于任何 `setState` 调用完成之后的操作。

```js
setState({ name: "sudheer" }, () => {
  console.log("name 参数已更新，组件已重新渲染")
})
```


#### 加分回答


* 回调函数在 `setState` 执行完之后调用，并且可以用于任何之后的操作。
* 推荐使用生命周期函数，而不是回调函数。


##### 相关链接


* [React docs on `setState`](https://reactjs.org/docs/react-component.html#setstate)

</details>

<br>[⬆ 回到顶部](#内容)

### JavaScript 里面表达式（Expression）和语句（Statement）的区别是什么？

<details>
<summary>查看答案</summary>

JavaScript 里面有两个主要的语法类别：表达式和语句。第三种语法是同时使用两者，称为表达式语句（Expression statement）。它们可以大致总结如下：

* **表达式（Expression）**: 产生一个值
* **语句（Statement）**: 执行一个操作
* **表达式语句（Expression statement）**: 产生一个值并且执行一个操作

经验法则:

> 如果你可以打印出来或者把它赋给一个变量，那么他是一个表达式。如果不能，那它是一个语句。

##### Statements

```js
let x = 0

function declaration() {}

if (true) {
}
```

语句执行操作，但是不产生值。

```js
// 将 `y` 的绝对值赋给 `x`
var x
if (y >= 0) {
  x = y
} else {
  x = -y
}
```

上面唯一的表达式是 `y >=0`，它产生了一个值，`true` 或者 `false`。值不是由代码的其他部分产生的。

##### Expressions

表达式产生一个值。他们可以被传到函数里面，因为解释器会用他们解析出来的值替换它们。

```js
5 + 5 // => 10

lastCharacter("input") // => "t"

true === true // => true
```

##### 表达式语句

通过使用条件运算符，可以将之前的语句集转化为一个等价的表达式。

```js
// 将 `y` 的绝对值赋给 `x`
var x = y >= 0 ? y : -y
```

这既是表达式也是语句，因为我们声明了一个变量 `x`（语句），其值为一个求值结果（表达式）


#### 加分回答


* 函数声明和函数表达式


##### 相关链接


* [声明和表达式的区别是什么？](https://stackoverflow.com/questions/12703214/javascript-difference-between-a-statement-and-an-expression)

</details>

<br>[⬆ 回到顶部](#内容)

### JavaScript 中的真值（Truthy）和假值（Falsy）是什么？

<details>
<summary>查看答案</summary>

一个值要么是真值要么是假值，取决于他在布尔上下文（Boolean context）中是如何被计算的。假值意味着似假的（False-like），真值意味着似真的（True-like）。本质上，这些值在执行某些操作时，会被强制类型转换为 `true` 或者 `false`。

JavaScript 中有 6 个假值。他们是：

* `false`
* `undefined`
* `null`
* `""` (空字符串)
* `NaN`
* `0` (`+0` 和 `-0`)

其他的值都被认为是真值。

一个值的真假性可以通过把其传入 `Boolean` 函数来检测。

```js
Boolean("") // false
Boolean([]) // true
```

逻辑非运算符 `!` 是一种检测真假性的快捷方式。使用 `!` 会讲一个值转换为其等价的布尔逆变换（例如，非假即为真），再做一次 `!` 会将其转换回来，通过这样的方式可以高效地讲一个值转换为布尔值。

```js
!!"" // false
!![] // true
```


#### 加分回答




##### 相关链接


* [Truthy on MDN](https://developer.mozilla.org/en/docs/Glossary/Truthy)
* [Falsy on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)

</details>

<br>[⬆ 回到顶部](#内容)

### 生成一个包含 n 项斐波那契数列的数组。

<details>
<summary>查看答案</summary>

初始化一个长度为 n 的空数组。使用 `Array.prototype.reduce()` 在数组中增加值，每个值都是前面最后两个值的和（除了最开始两个值）。

```js
const fibonacci = n =>
  [...Array(n)].reduce(
    (acc, val, i) => acc.concat(i > 1 ? acc[i - 1] + acc[i - 2] : i),
    []
  )
```


#### 加分回答




##### 相关链接


* [类似问题](https://github.com/Chalarangelo/30-seconds-of-code/blob/master/snippets_archive/fibonacciUntilNum.md)

</details>

<br>[⬆ 回到顶部](#内容)

### `0.1 + 0.2 === 0.3` 的值是什么？

<details>
<summary>查看答案</summary>

它的计算结果是 `false`，因为 JavaScript 的数学计算使用 IEEE 754 标准，并且使用了 64 位的浮点数。这造成了在进行小数运算时的精度问题，简而言之，这是因为计算机是基于二进制工作的，而小数是十进制的。

```js
0.1 + 0.2 // 0.30000000000000004
```

可以通过一个函数来判断两个数字是否大致相等来解决该问题。该函数定义一个误差值（Error margin），判断两个值的差值是否小于该误差值。

```js
const approxEqual = (n1, n2, epsilon = 0.0001) => Math.abs(n1 - n2) < epsilon
approxEqual(0.1 + 0.2, 0.3) // true
```


#### 加分回答


* 解决该问题的简单方法


##### 相关链接


* [一个检测相等性的简单辅助函数](https://github.com/Chalarangelo/30-seconds-of-code#approximatelyequal)
* [解决 JavaScript 中的 "0.1 + 0.2 = 0.300000004"](http://blog.blakesimpson.co.uk/read/61-fix-0-1-0-2-0-300000004-in-javascript)

</details>

<br>[⬆ 回到顶部](#内容)

### 数组方法 `map()` 和 `forEach()` 的区别是什么？

<details>
<summary>查看答案</summary>

两个方法都会变量数组的所有元素。`map()` 通过在每个元素上调用回调函数，从而将每个元素映射为一个新的元素，并返回一个新的数组。另一方面，`forEach()` 为每个元素调用回调函数，但是不返回一个新的数组。`forEach()` 通常被用于引发副作用的迭代，而 `map()` 通常用于函数式编程


#### 加分回答


* `forEach()` 用于以下场景：如果你需要对一个数组进行迭代，并且改变元素，同时不需要生成一个新的数组。
* `map()` 用于需要保持数据不可变的情况，此时所有的原数组中的数据都会被映射到一个新的数组中。


##### 相关链接


* [MDN docs for forEach](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
* [MDN docs for map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
* [JavaScript — Map vs. ForEach](https://codeburst.io/javascript-map-vs-foreach-f38111822c0f)

</details>

<br>[⬆ 回到顶部](#内容)

### What is short-circuit evaluation in JavaScript?

<details>
<summary>查看答案</summary>

Short-circuit evaluation involves logical operations evaluating from left-to-right and stopping early.

```js
true || false
```

In the above sample using logical OR, JavaScript won't look at the second operand `false`, because the expression evaluates to `true` regardless. This is known as short-circuit evaluation.

This also works for logical AND.

```js
false && true
```

This means you can have an expression that throws an error if evaluated, and it won't cause issues.

```js
true || nonexistentFunction()
false && nonexistentFunction()
```

This remains true for multiple operations because of left-to-right evaluation.

```js
true || nonexistentFunction() || window.nothing.wouldThrowError
true || window.nothing.wouldThrowError
true
```

A common use case for this behavior is setting default values. If the first operand is falsy the second operand will be evaluated.

```js
const options = {}
const setting = options.setting || "default"
setting // "default"
```

Another common use case is only evaluating an expression if the first operand is truthy.

```js
// Instead of:
addEventListener("click", e => {
  if (e.target.closest("button")) {
    handleButtonClick(e)
  }
})

// You can take advantage of short-circuit evaluation:
addEventListener(
  "click",
  e => e.target.closest("button") && handleButtonClick(e)
)
```

In the above case, if `e.target` is not or does not contain an element matching the `"button"` selector, the function will not be called. This is because the first operand will be falsy, causing the second operand to not be evaluated.


#### 加分回答


* Logical operations do not produce a boolean unless the operand(s) evaluate to a boolean.


##### 相关链接


* [JavaScript: What is short-circuit evaluation?](https://codeburst.io/javascript-what-is-short-circuit-evaluation-ff22b2f5608c)

</details>

<br>[⬆ 回到顶部](#内容)

### Are semicolons required in JavaScript?

<details>
<summary>查看答案</summary>

Sometimes. Due to JavaScript's automatic semicolon insertion, the interpreter places semicolons after most statements. This means semicolons can be omitted in most cases.

However, there are some cases where they are required. They are not required at the beginning of a block, but are if they follow a line and:

1.  The line starts with `[`

```js
const previousLine = 3
;[1, 2, previousLine].map(n => n * 2)
```

2.  The line starts with `(`

```js
const previousLine = 3
;(function() {
  // ...
})()
```

In the above cases, the interpreter does not insert a semicolon after `3`, and therefore it will see the `3` as attempting object property access or being invoked as a function, which will throw errors.


#### 加分回答


* Semicolons are usually optional in JavaScript but have edge cases where they are required.
* If you don't use semicolons, tools like Prettier will insert semicolons for you in the places where they are required on save in a text editor to prevent errors.


##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### 这个例子中，控制台会输出什么？

```js
var foo = 1
var foobar = function() {
  console.log(foo)
  var foo = 2
}
foobar()
```

<details>
<summary>查看答案</summary>

由于变量提升（Hoisting），局部变量会 `foo` 会在 `console.log` 调用之前声明。这意味着局部变量而不是全局变量的 `foo` 会作为一个参数被传入 `console.log`。然而，由于只有变量声明被提升，其值没有提升，所以输出会是 `undefined`，而不是 `2`。


#### 加分回答


* 变量提升是 JavaScript 的默认行为，会将声明移动到顶部。
* 提到严格（`strict`）模式。


##### 相关链接


* [MDN 文档：提升](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)

</details>

<br>[⬆ 回到顶部](#内容)

### JavaScript 中的变量提升（Hoisting）是如何工作的？

<details>
<summary>查看答案</summary>

变量提升是 JavaScript 的一种机制，变量和函数声明会在编译阶段被放到内存中去。这意味着，无论函数和变量在哪里被声明，也无论作用域是全局（global）还是局部（local），它们都会被移动到作用域的顶部，

然而，赋值是不会随着声明提升的。

以下代码段：

```js
console.log(hoist)
var hoist = "value"
```

和以下代码段等价：

```js
var hoist
console.log(hoist)
hoist = "value"
```

所以打印变量 `hoist` 会输出 `undefined` 而不是 `"value"`。

变量提升也允许你在一个函数声明（Function declaration）的位置之前调用一个函数。

```js
myFunction() // 没有错误; 打印 "hello"
function myFunction() {
  console.log("hello")
}
```

但是小心函数表达式（Function expression）有所不同：

```js
myFunction() // Error: `myFunction` is not a function
var myFunction = function() {
  console.log("hello")
}
```


#### 加分回答


* 变量提升是 JavaScript 的默认行为，其将变量提升到作用域顶部。
* 函数声明会被提升到变量声明之前。


##### 相关链接


* [MDN docs for hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)
* [理解 JavaScript 中的变量提升](https://scotch.io/tutorials/understanding-hoisting-in-javascript)

</details>

<br>[⬆ 回到顶部](#内容)

### HTML 和 React 的事件处理有什么区别？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* HTML 使用小写，React 使用驼峰。


##### 相关链接


* [React 文档：事件处理](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 回到顶部](#内容)

### 为什么要把整个 JavaScript 源文件包括在一个立即执行函数里面？

<details>
<summary>查看答案</summary>

这种方式在 JavaScript 里面很常见。它创建了一个包含了整个文件内容的闭包（closure），从而创建了一个私有的命名空间，进而避免了模块、库之间潜在的命名冲突。

```js
const myLibrary = (function() {
  var privateVariable = 2
  return {
    publicMethod: () => privateVariable
  }
})()
privateVariable // ReferenceError
myLibrary.publicMethod() // 2
```


#### 加分回答


* 在很多流行的 JavaScript 库中很流行。
* 创建了一个私有命名空间。


##### 相关链接


* [MDN 文档：闭包](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

</details>

<br>[⬆ 回到顶部](#内容)

### What does the following function return?

```js
function greet() {
  return
  {
    message: "hello"
  }
}
```

<details>
<summary>查看答案</summary>

Because of JavaScript's automatic semicolon insertion (ASI), the compiler places a semicolon after `return` keyword and therefore it returns `undefined` without an error being thrown.


#### 加分回答


* Automatic semicolon placement can lead to time-consuming bugs


##### 相关链接


* [Automatic semicolon insertion in JavaScript](http://2ality.com/2011/05/semicolon-insertion.html)

</details>

<br>[⬆ 回到顶部](#内容)

### 什么是内联条件表达式（Inline condition expression）？

<details>
<summary>查看答案</summary>

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


#### 加分回答




##### 相关链接


* [React 文档：条件渲染](https://reactjs.org/docs/conditional-rendering.html)

</details>

<br>[⬆ 回到顶部](#内容)

### Key 是什么？在列表里面使用它有什么好处？

<details>
<summary>查看答案</summary>

Key 是一种特殊的字符串属性，帮助 React 识别哪个元素改变、增加或者移除了。它们用于渲染数组时给它们一个稳定的标识。每一个元素的 key 都应该是独一无二的（比如数据中的 ID，或者最起码需要是序号）。

```js
const todoItems = todos.map(todo => <li key={todo.id}>{todo.text}</li>)
```

* 如果内容的顺序会改变，那么不推荐使用序号（Index）作为 key，因为这会降低性能并且引发组件的状态问题。
* 如果你把列表项提取出来作为一个组件，那么要把 key 使用在列表组件上，而不是 `<li>` 标签上。


#### 加分回答


* key 一个元素在集合中的稳定标识，并帮助 React 识别变化。
* 如果元素的顺序可能变化，那应该避免使用序号作为 key。
* 如果你把列表项提取出来成为组件，你应该将 key 应用在组件上，而不是 `<li>` 元素上。


##### 相关链接


* [React 文档：列表和 Key](https://reactjs.org/docs/lists-and-keys.html)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the difference between lexical scoping and dynamic scoping?

<details>
<summary>查看答案</summary>

Lexical scoping refers to when the location of a function's definition determines which variables you have access to. On the other hand, dynamic scoping uses the location of the function's invocation to determine which variables are available.


#### 加分回答


* Lexical scoping is also known as static scoping.
* Lexical scoping in JavaScript allows for the concept of closures.
* Most languages use lexical scoping because it tends to promote source code that is more easily understood.


##### 相关链接


* [Mozilla Docs Closures & Lexical Scoping](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

</details>

<br>[⬆ 回到顶部](#内容)

### Create a function that masks a string of characters with `#` except for the last four (4) characters.

```js
mask("123456789") // "#####6789"
```

<details>
<summary>查看答案</summary>

> There are many ways to solve this problem, this is just one one of them.

Using `String.prototype.slice()` we can grab the last 4 characters of the string by passing `-4` as an argument. Then, using `String.prototype.padStart()`, we can pad the string to the original length with the repeated mask character.

```js
const mask = (str, maskChar = "#") =>
  str.slice(-4).padStart(str.length, maskChar)
```


#### 加分回答


* Short, one-line functional solutions to problems should be preferred provided they are efficient


##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### What is the output of the following code?

```js
const a = [1, 2, 3]
const b = [1, 2, 3]
const c = "1,2,3"

console.log(a == c)
console.log(a == b)
```

<details>
<summary>查看答案</summary>

The first `console.log` outputs `true` because JavaScript's compiler performs type conversion and therefore it compares to strings by their value. On the other hand, the second `console.log` outputs `false` because Arrays are Objects and Objects are compared by reference.


#### 加分回答


* JavaScript performs automatic type conversion
* Objects are compared by reference
* Primitives are compared by value


##### 相关链接


* [JavaScript Value vs Reference](https://medium.com/dailyjs/back-to-roots-javascript-value-vs-reference-8fb69d587a18)

</details>

<br>[⬆ 回到顶部](#内容)

### How does prototypal inheritance differ from classical inheritance?

<details>
<summary>查看答案</summary>

In the classical inheritance paradigm, object instances inherit their properties and functions from a class, which acts as a blueprint for the object. Object instances are typically created using a constructor and the `new` keyword.

In the prototypal inheritance paradigm, object instances inherit directly from other objects and are typically created using factory functions or `Object.create()`.


#### 加分回答




##### 相关链接


* [MDN docs for inheritance and the prototype chain](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)

</details>

<br>[⬆ 回到顶部](#内容)

### What is a MIME type and what is it used for?

<details>
<summary>查看答案</summary>

`MIME` is an acronym for `Multi-purpose Internet Mail Extensions`. It is used as a standard way of classifying file types over the Internet.


#### 加分回答


* A `MIME type` actually has two parts: a type and a subtype that are separated by a slash (/). For example, the `MIME type` for Microsoft Word files is `application/msword` (i.e., type is application and the subtype is msword).


##### 相关链接


* [MIME Type MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)

</details>

<br>[⬆ 回到顶部](#内容)

### What are Promises?

<details>
<summary>查看答案</summary>

The `Promise` object represents the eventual completion (or failure) of an asynchronous operation, and its resulting value.
An example can be the following snippet, which after 100ms prints out the result string to the standard output. Also, note the catch, which can be used for error handling. `Promise`s are chainable.

```js
new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve("result")
  }, 100)
})
  .then(console.log)
  .catch(console.error)
```


#### 加分回答


* Take a look into the other questions regarding `Promise`s!


##### 相关链接


* [Master the JavaScript Interview: What is a Promise?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e772618)

</details>

<br>[⬆ 回到顶部](#内容)

### What are JavaScript data types?

<details>
<summary>查看答案</summary>

The latest ECMAScript standard defines seven data types, six of them being primitive: `Boolean`, `Null`, `Undefined`, `Number`, `String`, `Symbol` and one non-primitive data type: `Object`.


#### 加分回答


* Mention of newly added `Symbol` data type
* `Array`, `Date` and `function` are all of type `object`
* Functions in JavaScript are objects with the capability of being callable


##### 相关链接


* [MDN docs for data types and data structures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
* [Understanding Data Types in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-data-types-in-javascript)

</details>

<br>[⬆ 回到顶部](#内容)

### NodeJS often uses a callback pattern where if an error is encountered during execution, this error is passed as the first argument to the callback. What are the advantages of this pattern?

```js
fs.readFile(filePath, function(err, data) {
  if (err) {
    // handle the error, the return is important here
    // so execution stops here
    return console.log(err)
  }
  // use the data object
  console.log(data)
})
```

<details>
<summary>查看答案</summary>

Advantages include:

* Not needing to process data if there is no need to even reference it
* Having a consistent API leads to more adoption
* Ability to easily adapt a callback pattern that will lead to more maintainable code

As you can see from below example, the callback is called with null as its first argument if there is no error. However, if there is an error, you create an Error object, which then becomes the callback's only parameter. The callback function allows a user to easily know whether or not an error occurred.

This practice is also called the _Node.js error convention_, and this kind of callback implementations are called _error-first callbacks_.

```js
var isTrue = function(value, callback) {
  if (value === true) {
    callback(null, "Value was true.")
  } else {
    callback(new Error("Value is not true!"))
  }
}

var callback = function(error, retval) {
  if (error) {
    console.log(error)
    return
  }
  console.log(retval)
}

isTrue(false, callback)
isTrue(true, callback)

/*
  { stack: [Getter/Setter],
    arguments: undefined,
    type: undefined,
    message: 'Value is not true!' }
  Value was true.
*/
```


#### 加分回答


* This is just a convention. However, you should stick to it.


##### 相关链接


* [The Node.js Way Understanding Error-First Callbacks](http://fredkschott.com/post/2014/03/understanding-error-first-callbacks-in-node-js/)
* [What are the error conventions?](https://docs.nodejitsu.com/articles/errors/what-are-the-error-conventions)

</details>

<br>[⬆ 回到顶部](#内容)

### 什么是回调（Callback）？你可以举一个使用回调的例子吗？

<details>
<summary>查看答案</summary>

回调是作为参数传入其他函数的函数，并在一个事件发生或者特定的任务完成之后被调用，经常用于异步的代码。回调函数在之后被一段代码调用，但是可以在初始化阶段就声明而不必被调用。

例如，时间监听器作为异步的回调，只会在特定的事件发生时执行。

```js
function onClick() {
  console.log("用户点击了页面")
}
document.addEventListener("click", onClick)
```

然而，回调也可以是同步的。下面的 `map` 函数接受一个回调函数参数，该函数在循环的每次迭代（数组元素）中同步调用。

```js
const map = (arr, callback) => {
  const result = []
  for (let i = 0; i < arr.length; i++) {
    result.push(callback(arr[i], i))
  }
  return result
}
map([1, 2, 3, 4, 5], n => n * 2) // [2, 4, 6, 8, 10]
```


#### 加分回答


* 函数在 JavaScript 中是一等公民（First-class objects）
* 回调 vs Promise


##### 相关链接


* [MDN docs for callbacks](https://developer.mozilla.org/en-US/docs/Glossary/Callback_function)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the difference between `null` and `undefined`?

<details>
<summary>查看答案</summary>

In JavaScript, two values discretely represent nothing - `undefined` and `null`. The concrete difference between them is that `null` is explicit, while `undefined` is implicit. When a property does not exist or a variable has not been given a value, the value is `undefined`. `null` is set as the value to explicitly indicate “no value”. In essence, `undefined` is used when the nothing is not known, and `null` is used when the nothing is known.


#### 加分回答


* `typeof undefined` evaluates to `"undefined"`.
* `typeof null` evaluates `"object"`. However, it is still a primitive value and this is considered an implementation bug in JavaScript.
* `undefined == null` evaluates to `true`.


##### 相关链接


* [MDN docs for null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/null)
* [MDN docs for undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)

</details>

<br>[⬆ 回到顶部](#内容)

### Describe the different ways to create an object. When should certain ways be preferred over others?

<details>
<summary>查看答案</summary>

##### Object literal

Often used to store one occurrence of data.

```js
const person = {
  name: "John",
  age: 50,
  birthday() {
    this.age++
  }
}
person.birthday() // person.age === 51
```

##### Constructor

Often used when you need to create multiple instances of an object, each with their own data that other instances of the class cannot affect. The `new` operator must be used before invoking the constructor or the global object will be mutated.

```js
function Person(name, age) {
  this.name = name
  this.age = age
}
Person.prototype.birthday = function() {
  this.age++
}
const person1 = new Person("John", 50)
const person2 = new Person("Sally", 20)
person1.birthday() // person1.age === 51
person2.birthday() // person2.age === 21
```

##### Factory function

Creates a new object similar to a constructor, but can store private data using a closure. There is also no need to use `new` before invoking the function or the `this` keyword. Factory functions usually discard the idea of prototypes and keep all properties and methods as own properties of the object.

```js
const createPerson = (name, age) => {
  const birthday = () => person.age++
  const person = { name, age, birthday }
  return person
}
const person = createPerson("John", 50)
person.birthday() // person.age === 51
```

##### `Object.create()`

Sets the prototype of the newly created object.

```js
const personProto = {
  birthday() {
    this.age++
  }
}
const person = Object.create(personProto)
person.age = 50
person.birthday() // person.age === 51
```

A second argument can also be supplied to `Object.create()` which acts as a descriptor for the new properties to be defined.

```js
Object.create(personProto, {
  age: {
    value: 50,
    writable: true,
    enumerable: true
  }
})
```


#### 加分回答


* Prototypes are objects that other objects inherit properties and methods from.
* Factory functions offer private properties and methods through a closure but increase memory usage as a tradeoff, while classes do not have private properties or methods but reduce memory impact by reusing a single prototype object.


##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### What is the difference between a parameter and an argument?

<details>
<summary>查看答案</summary>

Parameters are the variable names of the function definition, while arguments are the values given to a function when it is invoked.

```js
function myFunction(parameter1, parameter2) {
  console.log(arguments[0]) // "argument1"
}
myFunction("argument1", "argument2")
```


#### 加分回答


* `arguments` is an array-like object containing information about the arguments supplied to an invoked function.
* `myFunction.length` describes the arity of a function (how many parameters it has, regardless of how many arguments it is supplied).


##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### Does JavaScript pass by value or by reference?

<details>
<summary>查看答案</summary>

JavaScript always passes by value. However, with objects, the value is a reference to the object.


#### 加分回答


* Difference between pass-by-value and pass-by-reference


##### 相关链接


* [JavaScript Value vs Reference](https://medium.com/dailyjs/back-to-roots-javascript-value-vs-reference-8fb69d587a18)

</details>

<br>[⬆ 回到顶部](#内容)

### How do you pass an argument to an event handler or callback?

<details>
<summary>查看答案</summary>

You can use an arrow function to wrap around an event handler and pass arguments, which is equivalent to calling `bind`:

```js
<button onClick={() => this.handleClick(id)} />
<button onClick={this.handleClick.bind(this, id)} />
```


#### 加分回答




##### 相关链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 回到顶部](#内容)

### What are fragments?

<details>
<summary>查看答案</summary>

Fragments allow a React component to return multiple elements without a wrapper, by grouping the children without adding extra elements to the DOM. Fragments offer better performance, lower memory usage, a cleaner DOM and can help in dealing with certain CSS mechanisms (e.g. tables, Flexbox and Grid).

```js
render() {
  return (
    <React.Fragment>
      <ChildA />
      <ChildB />
      <ChildC />
    </React.Fragment>
  );
}

// Short syntax supported by Babel 7
render() {
  return (
    <>
      <ChildA />
      <ChildB />
      <ChildC />
    </>
  );
}
```


#### 加分回答


* Fragments group multiple elements returned from a component, without adding a DOM element around them.


##### 相关链接


* [React docs on Fragments](https://reactjs.org/docs/fragments.html)

</details>

<br>[⬆ 回到顶部](#内容)

### Create a function `pipe` that performs left-to-right function composition by returning a function that accepts one argument.

```js
const square = v => v * v
const double = v => v * 2
const addOne = v => v + 1
const res = pipe(square, double, addOne)
res(3) // 19; addOne(double(square(3)))
```

<details>
<summary>查看答案</summary>

Gather all supplied arguments using the rest operator `...` and return a unary function that uses `Array.prototype.reduce()` to run the value through the series of functions before returning the final value.

```js
const pipe = (...fns) => x => fns.reduce((v, fn) => fn(v), x)
```


#### 加分回答


* Function composition is the process of combining two or more functions to produce a new function.


##### 相关链接


* [What is function composition?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-function-composition-20dfb109a1a0)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the event loop in Node.js?

<details>
<summary>查看答案</summary>

The event loop handles all async callbacks. Callbacks are queued in a loop, while other code runs, and will run one by one when the response for each one has been received.


#### 加分回答


* The event loop allows Node.js to perform non-blocking I/O operations, despite the fact that JavaScript is single-threaded


##### 相关链接


* [Node.js docs on event loop, timers and process.nextTick()](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the only value not equal to itself in JavaScript?

<details>
<summary>查看答案</summary>

`NaN` (Not-a-Number) is the only value not equal to itself when comparing with any of the comparison operators. `NaN` is often the result of meaningless math computations, so two `NaN` values make no sense to be considered equal.


#### 加分回答


* The difference between `isNaN()` and `Number.isNaN()`
* `const isNaN = x => x !== x`


##### 相关链接


* [MDN docs for `NaN`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN)

</details>

<br>[⬆ 回到顶部](#内容)

### Contrast mutable and immutable values, and mutating vs non-mutating methods.

<details>
<summary>查看答案</summary>

The two terms can be contrasted as:

* Mutable: subject to change
* Immutable: cannot change

In JavaScript, objects are mutable while primitive values are immutable. This means operations performed on objects can change the original reference in some way, while operations performed on a primitive value cannot change the original value.

All `String.prototype` methods do not have an effect on the original string and return a new string. On the other hand, while some methods of `Array.prototype` do not mutate the original array reference and produce a fresh array, some cause mutations.

```js
const myString = "hello!"
myString.replace("!", "") // returns a new string, cannot mutate the original value

const originalArray = [1, 2, 3]
originalArray.push(4) // mutates originalArray, now [1, 2, 3, 4]
originalArray.concat(4) // returns a new array, does not mutate the original
```


#### 加分回答


* List of mutating and non-mutating array methods


##### 相关链接


* [Mutating vs non-mutating array methods](https://lorenstewart.me/2017/01/22/javascript-array-methods-mutating-vs-non-mutating/)

</details>

<br>[⬆ 回到顶部](#内容)

### 什么是大 O 符号？

<details>
<summary>查看答案</summary>

大 O 符号用于在计算机科学中描述一个算法的时间复杂度。最好的算法会执行得最快，并且拥有最低的复杂性。

算法并不总是表现得相同，并且会根据所提供的数据而变化。尽管在某些情况下他们会执行得很快，在其他情况下他们会执行得很慢，即使他们处理了相同数量的元素。

在这些例子中，基础时间是 1 个元素 = `1ms`

##### O(1)

```js
arr[arr.length - 1]
```

* 1000 个元素 = `1ms`

常数时间复杂度。不管数组有多少个元素，理论上他们执行时间是相同的（排除实际的变化）。

##### O(N)

```js
arr.filter(fn)
```

* 1000 个元素 = `1000ms`

线性时间复杂度。执行时间会随着数组元素的数量线性地增长。如果数组有 1000 个元素并且函数执行一次花费 1ms，7000 个元素会执行 7ms。这是因为函数必须在返回结果之前遍历数组的所有元素。

##### O([1, N])

```js
arr.some(fn)
```

* 1000 个元素 = `1ms <= x <= 1000ms`

执行时间会根据提供的数据的不同而不同，函数可以很快活着很慢地返回。最好的情况是 O(1)，而最坏的情况是 O(N)。

##### O(NlogN)

```js
arr.sort(fn)
```

* 1000 elements ~= `10000ms`

浏览器通常为 `sort()` 方法实现了了快速排序（Quicksort），快排的平均时间复杂度是 O(NlgN)。这对大量数据非常高效。

##### O(N^2)

```js
for (let i = 0; i < arr.length; i++) {
  for (let j = 0; j < arr.length; j++) {
    // ...
  }
}
```

* 1000 个元素 = `1000000ms`

执行时间随着元素的数量平方增长。通常是由于嵌套的循环。

##### O(N!)

```js
const permutations = arr => {
  if (arr.length <= 2) return arr.length === 2 ? [arr, [arr[1], arr[0]]] : arr
  return arr.reduce(
    (acc, item, i) =>
      acc.concat(
        permutations([...arr.slice(0, i), ...arr.slice(i + 1)]).map(val => [
          item,
          ...val
        ])
      ),
    []
  )
}
```

* 1000 个元素 = `无限大（Infinity）` (实际上) ms

执行时间会增长地非常快，即使数组只增加了一个元素。


#### 加分回答


* 当执行时间呈指数增长时，要小心嵌套循环。


##### 相关链接


* [JavaScript 的大 O 符号](https://medium.com/cesars-tech-insights/big-o-notation-javascript-25c79f50b19b)

</details>

<br>[⬆ 回到顶部](#内容)

### What is a pure function?

<details>
<summary>查看答案</summary>

A pure function is a function that satisfies these two conditions:

* Given the same input, the function returns the same output.
* The function doesn't cause side effects outside of the function's scope (i.e. mutate data outside the function or data supplied to the function).

Pure functions can mutate local data within the function as long as it satisfies the two conditions above.

##### Pure

```js
const a = (x, y) => x + y
const b = (arr, value) => arr.concat(value)
const c = arr => [...arr].sort((a, b) => a - b)
```

##### Impure

```js
const a = (x, y) => x + y + Math.random()
const b = (arr, value) => (arr.push(value), arr)
const c = arr => arr.sort((a, b) => a - b)
```


#### 加分回答


* Pure functions are easier to reason about due to their reliability.
* All functions should be pure unless explicitly causing a side effect (i.e. `setInnerHTML`).
* If a function does not return a value, it is an indication that it is causing side effects.


##### 相关链接


* [Pure functions in JavaScript](http://www.nicoespeon.com/en/2015/01/pure-functions-javascript/)

</details>

<br>[⬆ 回到顶部](#内容)

### What is recursion and when is it useful?

<details>
<summary>查看答案</summary>

Recursion is the repeated application of a process. In JavaScript, recursion involves functions that call themselves repeatedly until they reach a base condition. The base condition breaks out of the recursion loop because otherwise the function would call itself indefinitely. Recursion is very useful when working with data structures that contain nesting where the number of levels deep is unknown.

For example, you may have a thread of comments returned from a database that exist in a flat array but need to be nested for display in the UI. Each comment is either a top-level comment (no parent) or is a reply to a parent comment. Comments can be a reply of a reply of a reply... we have no knowledge beforehand the number of levels deep a comment may be. This is where recursion can help.

```js
const nest = (items, id = null, link = "parent_id") =>
  items
    .filter(item => item[link] === id)
    .map(item => ({ ...item, children: nest(items, item.id) }))

const comments = [
  { id: 1, parent_id: null, text: "First reply to post." },
  { id: 2, parent_id: 1, text: "First reply to comment #1." },
  { id: 3, parent_id: 1, text: "Second reply to comment #1." },
  { id: 4, parent_id: 3, text: "First reply to comment #3." },
  { id: 5, parent_id: 4, text: "First reply to comment #4." },
  { id: 6, parent_id: null, text: "Second reply to post." }
]

nest(comments)
/*
[
  { id: 1, parent_id: null, text: "First reply to post.", children: [...] },
  { id: 6, parent_id: null, text: "Second reply to post.", children: [] }
]
*/
```

In the above example, the base condition is met if `filter()` returns an empty array. The chained `map()` won't invoke the callback function which contains the recursive call, thereby breaking the loop.


#### 加分回答


* Recursion is useful when working with data structures containing an unknown number of nested structures.
* Recursion must have a base condition to be met that breaks out of the loop or it will call itself indefinitely.


##### 相关链接


* [In plain English, what is recursion?](https://softwareengineering.stackexchange.com/questions/25052/in-plain-english-what-is-recursion)

</details>

<br>[⬆ 回到顶部](#内容)

### What is memoization?

<details>
<summary>查看答案</summary>

Memoization is the process of caching the output of function calls so that subsequent calls are faster. Calling the function again with the same input will return the cached output without needing to do the calculation again.

A basic implementation in JavaScript looks like this:

```js
const memoize = fn => {
  const cache = new Map()
  return value => {
    const cachedResult = cache.get(value)
    if (cachedResult !== undefined) return cachedResult
    const result = fn(value)
    cache.set(value, result)
    return result
  }
}
```


#### 加分回答


* The above technique returns a unary function even if the function can take multiple arguments.
* The first function call will be slower than usual because of the overhead created by checking if a cached result exists and setting a result before returning the value.
* Memoization increases performance on subsequent function calls but still needs to do work on the first call.


##### 相关链接


* [Implementing memoization in JavaScript](https://www.sitepoint.com/implementing-memoization-in-javascript/)

</details>

<br>[⬆ 回到顶部](#内容)

### What are refs in React? When should they be used?

<details>
<summary>查看答案</summary>

Refs provide a way to access DOM nodes or React elements created in the render method. Refs should be used sparringly, but there are some good use cases for refs, such as:

* Managing focus, text selection, or media playback.
* Triggering imperative animations.
* Integrating with third-party DOM libraries.

Refs are created using `React.createRef()` method and attached to React elements via the `ref` attribute. In order to use refs throughout the component, assign the `ref` to the instance property within the constructor:

```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props)
    this.myRef = React.createRef()
  }

  render() {
    return <div ref={this.myRef} />
  }
}
```

Refs can also be used in functional components with the help of closures.


#### 加分回答


* Refs are used to return a reference to an element.
* Refs shouldn't be overused.
* You can create a ref using `React.createRef()` and attach to elements via the `ref` attribute.


##### 相关链接


* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html)

</details>

<br>[⬆ 回到顶部](#内容)

### Explain the differences between imperative and declarative programming.

<details>
<summary>查看答案</summary>

These two types of programming can roughly be summarized as:

* Imperative: **how** to achieve something
* Declarative: **what** should be achieved

A common example of declarative programming is CSS. The developer specifies CSS properties that describe what something should look like rather than how to achieve it. The "how" is abstracted away by the browser.

On the other hand, imperative programming involves the steps required to achieve something. In JavaScript, the differences can be contrasted like so:

##### Imperative

```js
const numbers = [1, 2, 3, 4, 5]
const numbersDoubled = []
for (let i = 0; i < numbers.length; i++) {
  numbersDoubled[i] = numbers[i] * 2
}
```

We manually loop over the numbers of the array and assign the new index as the number doubled.

##### Declarative

```js
const numbers = [1, 2, 3, 4, 5]
const numbersDoubled = numbers.map(n => n * 2)
```

We declare that the new array is mapped to a new one where each value is doubled.


#### 加分回答


* Declarative programming often works with functions and expressions. Imperative programming frequently uses statements and relies on low-level features that cause mutations, while declarative programming has a strong focus on abstraction and purity.
* Declarative programming is more terse and easier to process at a glance.


##### 相关链接


* [Declarative vs Imperative Programming](https://codeburst.io/declarative-vs-imperative-programming-a8a7c93d9ad2)

</details>

<br>[⬆ 回到顶部](#内容)

### What is functional programming?

<details>
<summary>查看答案</summary>

Functional programming is a paradigm in which programs are built in a declarative manner using pure functions that avoid shared state and mutable data. Functions that always return the same value for the same input and don't produce side effects are the pillar of functional programming. Many programmers consider this to be the best approach to software development as it reduces bugs and cognitive load.


#### 加分回答


* Cleaner, more concise development experience
* Simple function composition
* Features of JavaScript that enable functional programming (`.map`, `.reduce` etc.)
* JavaScript is multi-paradigm programming language (Object-Oriented Programming and Functional Programming live in harmony)


##### 相关链接


* [Javascript and Functional Programming: An Introduction](https://hackernoon.com/javascript-and-functional-programming-an-introduction-286aa625e26d)
* [Master the JavaScript Interview: What is Functional Programming?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)

</details>

<br>[⬆ 回到顶部](#内容)

### What are portals in React?

<details>
<summary>查看答案</summary>

Portal are the recommended way to render children into a DOM node that exists outside the DOM hierarchy of the parent component.

```js
ReactDOM.createPortal(child, container)
```

The first argument (`child`) is any renderable React child, such as an element, string, or fragment. The second argument (`container`) is a DOM element.


#### 加分回答




##### 相关链接


* [React docs on Portals](https://reactjs.org/docs/portals.html)

</details>

<br>[⬆ 回到顶部](#内容)

### 什么是事件驱动编程？

<details>
<summary>查看答案</summary>

时间驱动编程是一种范式，它涉及到构建一个发送和接收事件的应用。当程序发送事件的时候，程序会通过执行所有注册在这个事件上的回调函数，并将相关数据传入该函数。使用这种模式，即便没有函数订阅该事件，也可以将事件释放到外部而不引发错误。

一个通常的例子是，元素监听 DOM 事件，比如 `click` 和 `mouseenter`，当事件发生时，回调函数会被运行。

```js
document.addEventListener("click", function(event) {
  // This callback function is run when the user
  // clicks on the document.
})
```

在没有 DOM 上下文（context）的情况下，该模式可能是这样的：

```js
const hub = createEventHub()
hub.on("message", function(data) {
  console.log(`${data.username} said ${data.text}`)
})
hub.emit("message", {
  username: "John",
  text: "Hello?"
})
```

在这种实现中，`on` 是*订阅*一个事件的方法，`emit` 是*发布*一个事件的方法。


#### 加分回答


* 遵循发布-订阅（publish-subscribe）模式。
* 通过执行所有订阅该事件的回调函数来响应该事件。
* 展示如何用 JavaScript 创建一个简单的发布-订阅模式。


##### 相关链接


* [MDN 文档：事件和处理器](https://developer.mozilla.org/en-US/docs/Web/Guide/Events/Overview_of_Events_and_Handlers)
* [理解 Node.js 的事件驱动（event-driven）架构](https://medium.freecodecamp.org/understanding-node-js-event-driven-architecture-223292fcbc2d)

</details>

<br>[⬆ 回到顶部](#内容)

### 什么是上下文（Context）？

<details>
<summary>查看答案</summary>

上下文提供了一种通过组件树传递数据的方式，而不需要手动地在每层把参数传递下去。比如，授权的用户、语言信息、UI 主题这些需要被应用中的很多组件获取的数据。

```js
const { Provider, Consumer } = React.createContext(defaultValue)
```


#### 加分回答


* 上下文提供了一个在 React 组件树中传递数据的方式，而不需要手动地传递参数。
* 上下文被设计用来在 React 组件树中共享可以被视为*全局*的数据。


##### 相关链接


* [React 文档：上下文](https://reactjs.org/docs/context.html)

</details>

<br>[⬆ 回到顶部](#内容)

### Explain the difference between a static method and an instance method.

<details>
<summary>查看答案</summary>

Static methods belong to a class and don't act on instances, while instance methods belong to the class prototype which is inherited by all instances of the class and acts on them.

```js
Array.isArray // static method of Array
Array.prototype.push // instance method of Array
```

In this case, the `Array.isArray` method does not make sense as an instance method of arrays because we already know the value is an array when working with it.

Instance methods could technically work as static methods, but provide terser syntax:

```js
const arr = [1, 2, 3]
arr.push(4)
Array.push(arr, 4)
```


#### 加分回答


* How to create static and instance methods with ES2015 class syntax


##### 相关链接


* [Classes on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

</details>

<br>[⬆ 回到顶部](#内容)

### 闭包（closure）是什么？你可以给一个有用的例子嘛？

<details>
<summary>查看答案</summary>

闭包是一个定义在其他函数里面的函数，并且有权访问其词法作用域（lexical scope）—— 甚至于当它在运行在其词法作用域以外的时候。闭包有权访问以下三个作用域的变量：

* 定义在其自身作用域的变量
* 定义在其父函数作用域的变量
* 定义在全局作用域的变量

在 JavaScript，所有的函数都是闭包，因为他们有权限访问外部的作用域，但是大部分函数没有充分利用闭包的特性：状态保存。这也是为什么闭包有时候被称为状态函数（stateful function）

另外，闭包也是 JavaScript 里面唯一的保存外部无法访问的私有数据的方式。这是 UMD（Universal Module Definition）模式的关键，经常用于库里面，可以让库只暴露公开 API，但是让其实现细节（implementation detail）保持私密，避免了和其他库或者用户的代码的命名冲突。


#### 加分回答


* 闭包非常有用，因为它允许你将数据和操作该数据的函数关联起来。
* 一个闭包可以用一个函数替代一个对象。
* 闭包可以用于模拟私有属性和方法。


##### 相关链接


* [MDN docs for closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)
* [什么是闭包](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36)
* [我从未理解 JavaScript 的闭包](https://medium.com/dailyjs/i-never-understood-javascript-closures-9663703368e8)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the `this` keyword and how does it work?

<details>
<summary>查看答案</summary>

The `this` keyword is an object that represents the context of an executing function. Regular functions can have their `this` value changed with the methods `call()`, `apply()` and `bind()`. Arrow functions implicitly bind `this` so that it refers to the context of its lexical environment, regardless of whether or not its context is set explicitly with `call()`.

Here are some common examples of how `this` works:

##### Object literals

`this` refers to the object itself inside regular functions if the object precedes the invocation of the function.

Properties set as `this` do not refer to the object.

```js
var myObject = {
  property: this,
  regularFunction: function() {
    return this
  },
  arrowFunction: () => {
    return this
  },
  iife: (function() {
    return this
  })()
}
myObject.regularFunction() // myObject
myObject["regularFunction"]() // my Object

myObject.property // NOT myObject; lexical `this`
myObject.arrowFunction() // NOT myObject; lexical `this`
myObject.iife // NOT myObject; lexical `this`
const regularFunction = myObject.regularFunction
regularFunction() // NOT myObject; lexical `this`
```

##### Event listeners

`this` refers to the element listening to the event.

```js
document.body.addEventListener("click", function() {
  console.log(this) // document.body
})
```

##### Constructors

`this` refers to the newly created object.

```js
class Example {
  constructor() {
    console.log(this) // myExample
  }
}
const myExample = new Example()
```

##### Manual

With `call()` and `apply()`, `this` refers to the object passed as the first argument.

```js
var myFunction = function() {
  return this
}
myFunction.call({ customThis: true }) // { customThis: true }
```

##### Unwanted `this`

Because `this` can change depending on the scope, it can have unexpected values when using regular functions.

```js
var obj = {
  arr: [1, 2, 3],
  doubleArr() {
    return this.arr.map(function(value) {
      // this is now this.arr
      return this.double(value)
    })
  },
  double() {
    return value * 2
  }
}
obj.doubleArr() // Uncaught TypeError: this.double is not a function
```


#### 加分回答


* In non-strict mode, global `this` is the global object (`window` in browsers), while in strict mode global `this` is `undefined`.
* `Function.prototype.call` and `Function.prototype.apply` set the `this` context of an executing function as the first argument, with `call` accepting a variadic number of arguments thereafter, and `apply` accepting an array as the second argument which are fed to the function in a variadic manner.
* `Function.prototype.bind` returns a new function that enforces the `this` context as the first argument which cannot be changed by other functions.
* If a function requires its `this` context to be changed based on how it is called, you must use the `function` keyword. Use arrow functions when you want `this` to be the surrounding (lexical) context.


##### 相关链接


* [`this` on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)

</details>

<br>[⬆ 回到顶部](#内容)

### `children` 参数是什么？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* 子元素（Children）是一个允许组件像数据一样被传递给其他组件的参数。
* React API 提供了使用这个属性的方法。


##### 相关链接


* [React docs on Children](https://reactjs.org/docs/jsx-in-depth.html#children-in-jsx)

</details>

<br>[⬆ 回到顶部](#内容)

### 回调引用（callback refs） 和 findDOMNode()，哪个更好？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* 更推荐使用回调引用而不是 `findDOMNode()`。


##### 相关链接


* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html#exposing-dom-refs-to-parent-components)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the purpose of JavaScript UI libraries/frameworks like React, Vue, Angular, Hyperapp, etc?

<details>
<summary>查看答案</summary>

The main purpose is to avoid manipulating the DOM directly and keep the state of an application
in sync with the UI easily. Additionally, they provide the ability to create components that can be reused when they have similar functionality with minor differences, avoiding duplication which would require multiple changes whenever the structure of a component which is reused in multiple places needs to be updated.

When working with DOM manipulation libraries like jQuery, the data of an application is generally kept in the DOM itself, often as class names or `data` attributes. Manipulating the DOM to update the UI involves many extra steps and can introduce subtle bugs over time. Keeping the state separate and letting a framework handle the UI updates when the state changes reduces cognitive load. Saying you want the UI to look a certain way when the state is a certain value is the declarative way of creating an application, instead of the imperative way of manually updating the UI to reflect the new state.


#### 加分回答


* The virtual DOM is a representation of the real DOM tree in the form of plain objects, which allows a library to write code as if the entire document is thrown away and rebuilt on each change, while the real DOM only updates what needs to be changed. Comparing the new virtual DOM against the previous one leads to high efficiency as changing real DOM nodes is costly compared to recalculating the virtual DOM.
* JSX is an extension to JavaScript that provides XML-like syntax to create virtual DOM objects which is transformed to function calls by a transpiler. It simplifies control flow (if statements/ternary expressions) compared to tagged template literals.


##### 相关链接


* [Virtual DOM in Hyperapp](https://github.com/hyperapp/hyperapp#view)

</details>

<br>[⬆ 回到顶部](#内容)

### What does `'use strict'` do and what are some of the key benefits to using it?

<details>
<summary>查看答案</summary>

Including `'use strict'` at the beginning of your JavaScript source file enables strict mode, which enforces more strict parsing and error handling of JavaScript code. It is considered a good practice and offers a lot of benefits, such as:

* Easier debugging due to eliminating silent errors.
* Disallows variable redefinition.
* Prevents accidental global variables.
* Oftentimes provides increased performance over identical code that is not running in strict mode.
* Simplifies `eval()` and `arguments`.
* Helps make JavaScript more secure.


#### 加分回答


* Eliminates `this` coercion, throwing an error when `this` references a value of `null` or `undefined`.
* Throws an error on invalid usage of `delete`.
* Prohibits some syntax likely to be defined in future versions of ECMAScript


##### 相关链接


* [MDN docs for strict mode](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode)

</details>

<br>[⬆ 回到顶部](#内容)

### 如何避免回调地狱？

```js
getData(function(a) {
  getMoreData(a, function(b) {
    getMoreData(b, function(c) {
      getMoreData(c, function(d) {
        getMoreData(d, function(e) {
          // ...
        })
      })
    })
  })
})
```

<details>
<summary>查看答案</summary>

一般最好的方式是用 `async/await` 将函数重构，使其返回一个 promise。相比较于给函数传递一个回调而造成深层的嵌套，这种方式可以返回一个可以用于 `await` 的 promise，并且可以在数据一返回就被处理，而下一行代码也可以以一种类似同步（sync-like）的方式执行。

上面的代码可以被重构如下：

```js
async function asyncAwaitVersion() {
  const a = await getData()
  const b = await getMoreData(a)
  const c = await getMoreData(b)
  const d = await getMoreData(c)
  const e = await getMoreData(d)
  // ...
}
```

有很多可以解决回调地狱的方法：

* 模块化（Modularization）：将回调拆分成独立的函数。
* 使用一个流程控制库，比如 async。
* 搭配 generator 使用 promise。
* 使用 async/await （node v7 以上）。


#### 加分回答


* 作为一个高效的 JavaScript 开发者，你必须要避免不断增长的缩进级别，要书写干净且可读的代码，并且可以处理复杂的流程。


##### 相关链接


* [避免 Node.js 中的回调地狱](http://stackabuse.com/avoiding-callback-hell-in-node-js/)
* [异步 JavaScript：从 Callback 到 Async、Await](https://blog.hellojs.org/asynchronous-javascript-from-callback-hell-to-async-and-await-9b9ceb63c8e8)

</details>

<br>[⬆ 回到顶部](#内容)

### What is a virtual DOM and why is it used in libraries/frameworks?

<details>
<summary>查看答案</summary>

The virtual DOM (VDOM) is a representation of the real DOM in the form of plain JavaScript objects. These objects have properties to describe the real DOM nodes they represent: the node name, its attributes, and child nodes.

```html
<div class="counter">
  <h1>0</h1>
  <button>-</button>
  <button>+</button>
</div>
```

The above markup's virtual DOM representation might look like this:

```js
{
  nodeName: "div",
  attributes: { class: "counter" },
  children: [
    {
      nodeName: "h1",
      attributes: {},
      children: [0]
    },
    {
      nodeName: "button",
      attributes: {},
      children: ["-"]
    },
    {
      nodeName: "button",
      attributes: {},
      children: ["+"]
    }
  ]
}
```

The library/framework uses the virtual DOM as a means to improve performance. When the state of an application changes, the real DOM needs to be updated to reflect it. However, changing real DOM nodes is costly compared to recalculating the virtual DOM. The previous virtual DOM can be compared to the new virtual DOM very quickly in comparison.

Once the changes between the old VDOM and new VDOM have been calculated by the diffing engine of the framework, the real DOM can be patched efficiently in the least time possible to match the new state of the application.


#### 加分回答


* Why accessing the DOM can be so costly.


##### 相关链接


* [The difference between Virtual DOM and DOM](http://reactkungfu.com/2015/10/the-difference-between-virtual-dom-and-dom/)

</details>

<br>[⬆ 回到顶部](#内容)

### How do you ensure methods have the correct `this` context in React component classes?

<details>
<summary>查看答案</summary>

In JavaScript classes, the methods are not bound by default. This means that their `this` context can be changed (in the case of an event handler, to the element that is listening to the event) and will not refer to the component instance. To solve this, `Function.prototype.bind()` can be used to enforce the `this` context as the component instance.

```js
constructor(props) {
  super(props);
  this.handleClick = this.handleClick.bind(this);
}

handleClick() {
  // Perform some logic
}
```

* The `bind` approach can be verbose and requires defining a `constructor`, so the new public class fields syntax is generally preferred:

```js
handleClick = () => {
  console.log('this is:', this);
}

render() {
  return (
    <button onClick={this.handleClick}>
      Click me
    </button>
  );
}
```

* You can also use an inline arrow function, because lexical `this` (referring to the component instance) is preserved:

```js
<button onClick={e => this.handleClick(e)}>Click me</button>
```

Note that extra re-rendering can occur using this technique because a new function reference is created on render, which gets passed down to child components and breaks `shouldComponentUpdate` / `PureComponent` shallow equality checks to prevent unnecessary re-renders. In cases where performance is important, it is preferred to go with `bind` in the constructor, or the public class fields syntax approach, because the function reference remains constant.


#### 加分回答


* You can either bind methods to the component instance context in the constructor, use public class fields syntax, or use inline arrow functions.


##### 相关链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)
* [React docs on Passing Functions to Components](https://reactjs.org/docs/faq-functions.html#how-do-i-bind-a-function-to-a-component-instance)

</details>

<br>[⬆ 回到顶部](#内容)


## React
### 无状态组件是什么？

<details>
<summary>查看答案</summary>

无状态组件的行为不依赖于自身的状态。无状态组件可以是函数组件或者类组件。无状态函数组件更方便维护和测试，因为他们会保证在相同的参数下生成相同的输出。在没有用到生命周期钩子（Hooks）的情况下，应该优先使用无状态函数组件。


#### 加分回答


* 无状态组件独立于他们的状态。
* 无状态组件可以是类组件或函数式组件。
* 无状态函数组件应该完全避免使用 `this` 关键词。


##### 相关链接


* [React 文档 状态和生命周期](https://reactjs.org/docs/state-and-lifecycle.html)

</details>

<br>[⬆ 回到顶部](#内容)

### React 中的有状态组件（Stateful Component）是什么意思？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* 有状态组件具有它们依赖的内部状态。
* 有状态组件包括类组件和使用了有状态 Hooks 的函数组件。
* 有状态组件在他们的构造函数（constructor）里面或者用 `useState()` 来初始化状态。


##### 相关链接


* [React 文档 状态和生命周期](https://reactjs.org/docs/state-and-lifecycle.html)

</details>

<br>[⬆ 回到顶部](#内容)

### How do you write comments inside a JSX tree in React?

<details>
<summary>查看答案</summary>

Comments must be wrapped inside curly braces `{}` and use the `/* */` syntax.

```jsx
const tree = (
  <div>
    {/* Comment */}
    <p>Text</p>
  </div>
)
```

<!-- tags: (react) -->

<!-- expertise: (0) -->


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### React 中元素（Element）和组件（Component）的区别是什么？

<details>
<summary>查看答案</summary>

元素是一个纯 JavaScript 对象，代表了一个 DOM 节点或者组件。元素是纯粹的、不可变的，并且创建消耗低。

一个组件是一个函数或者类（Class）。组件可以有状态，接收参数（props），并且返回一个元素树（尽管他们可以表示一个通用的容器或者包装器，并且不一定必须要生成 DOM）。组件可以在生命周期方法里面触发副作用（Side effects），比如 AJAX 请求、DOM 变动、调用第三方库，并且创建可能会很昂贵。

```js
const Component = () => "Hello"
const componentElement = <Component />
const domNodeElement = <div />
```


#### 加分回答


* 元素是不可变的纯对象，描述了你要创建的 DOM 节点或者组件。
* 组件可以是类或者函数，接收参数并且返回元素树（Element Tree）


##### 相关链接


* [React docs on Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
* [React docs on Components and Props](https://reactjs.org/docs/components-and-props.html)

</details>

<br>[⬆ 回到顶部](#内容)

### What does lifting state up in React mean?

<details>
<summary>查看答案</summary>

When several components need to share the same data, then it is recommended to lift the shared state up to their closest common ancestor. For example, if two child components share the same data, it is recommended to move the shared state to parent instead of maintaining the local state in both child components.


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### Why does React use `className` instead of `class` like in HTML?

<details>
<summary>查看答案</summary>

React's philosophy in the beginning was to align with the browser DOM API rather than HTML, since that more closely represents how elements are created. Setting a `class` on an element meant using the `className` API:

```js
const element = document.createElement("div")
element.className = "hello"
```

Additionally, before ES5, reserved words could not be used in objects:

```js
const element = {
  attributes: {
    class: "hello"
  }
}
```

In IE8, this will throw an error.

In modern environments, destructuring will throw an error if trying to assign to a variable:

```js
const { class } = this.props // Error
const { className } = this.props // All good
const { class: className } = this.props // All good, but cumbersome!
```

However, `class` _can_ be used as a prop without problems, as seen in other libraries like Preact. React currently allows you to use `class`, but will throw a warning and convert it to `className` under the hood. There is currently an open thread (as of January 2019) discussing changing `className` to `class` to reduce confusion.


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### How do you pass an argument to an event handler or callback?

<details>
<summary>查看答案</summary>

You can use an arrow function to wrap around an event handler and pass arguments, which is equivalent to calling `bind`:

```js
<button onClick={() => this.handleClick(id)} />
<button onClick={this.handleClick.bind(this, id)} />
```


#### 加分回答




##### 相关链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 回到顶部](#内容)

### `setState` 的回调函数（Callback function）参数有什么用？

<details>
<summary>查看答案</summary>

回调函数在 `setState` 执行完毕，并且组件渲染完毕之后调用。由于 `setState` 是异步的，回调函数可以用于任何 `setState` 调用完成之后的操作。

```js
setState({ name: "sudheer" }, () => {
  console.log("name 参数已更新，组件已重新渲染")
})
```


#### 加分回答


* 回调函数在 `setState` 执行完之后调用，并且可以用于任何之后的操作。
* 推荐使用生命周期函数，而不是回调函数。


##### 相关链接


* [React docs on `setState`](https://reactjs.org/docs/react-component.html#setstate)

</details>

<br>[⬆ 回到顶部](#内容)

### What are the different phases of the component lifecycle in React?

<details>
<summary>查看答案</summary>

There are four different phases of component’s lifecycle:

**Initialization**: In this phase, the component prepares setting up the initial state and default props.

**Mounting**: The react component is ready to mount to the DOM. This phase covers the `getDerivedStateFromProps` and `componentDidMount` lifecycle methods.

**Updating**: In this phase, the component gets updated in two ways, sending the new props and updating the state. This phase covers the `getDerivedStateFromProps`, `shouldComponentUpdate`, `getSnapshotBeforeUpdate` and `componentDidUpdate` lifecycle methods.

**Unmounting**: In this last phase, the component is not needed and gets unmounted from the browser DOM. This phase includes the `componentWillUnmount` lifecycle method.

**Error Handling**: In this phase, the component is called whenever there's an error during rendering, in a lifecycle method, or in the constructor for any child component. This phase includes the `componentDidCatch` lifecycle method.

<img alt="lifecycle phases" src="https://pbs.twimg.com/media/DZ-97vzW4AAbcZj.jpg:large" style="width: 100%"/>


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### HTML 和 React 的事件处理有什么区别？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* HTML 使用小写，React 使用驼峰。


##### 相关链接


* [React 文档：事件处理](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 回到顶部](#内容)

### 什么是内联条件表达式（Inline condition expression）？

<details>
<summary>查看答案</summary>

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


#### 加分回答




##### 相关链接


* [React 文档：条件渲染](https://reactjs.org/docs/conditional-rendering.html)

</details>

<br>[⬆ 回到顶部](#内容)

### What are the lifecycle methods in React?

<details>
<summary>查看答案</summary>

`getDerivedStateFromProps`: Executed before rendering on the initial mount and all component updates. Used to update the state based on changes in props over time. Has rare use cases, like tracking component animations during the lifecycle. There are only few cases where this makes sense to use over other lifecycle methods. It expects to return an object that will be the the new state, or null to update nothing. This method does not have access to the component instance either.

`componentDidMount`: Executed after first rendering and here all AJAX requests, DOM or state updates, and set up eventListeners should occur.

`shouldComponentUpdate`: Determines if the component will be updated or not. By default, it returns true. If you are sure that the component doesn't need to render after state or props are updated, you can return a false value. It is a great place to improve performance as it allows you to prevent a rerender if component receives new prop.

`getSnapshotBeforeUpdate`: Invoked right after a component render happens because of an update, before `componentDidUpdate`. Any value returned from this method will be passed to `componentDidUpdate`.

`componentDidUpdate`: Mostly it is used to update the DOM in response to prop or state changes.

`componentWillUnmount`: It will be used to cancel any outgoing network requests, or remove all event listeners associated with the component.

`componentDidCatch`: Used in error boundaries, which are components that implement this method. It allows the component to catch JavaScript errors anywhere in the _child_ component tree (below this component), log errors, and display a UI with error information.


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### Key 是什么？在列表里面使用它有什么好处？

<details>
<summary>查看答案</summary>

Key 是一种特殊的字符串属性，帮助 React 识别哪个元素改变、增加或者移除了。它们用于渲染数组时给它们一个稳定的标识。每一个元素的 key 都应该是独一无二的（比如数据中的 ID，或者最起码需要是序号）。

```js
const todoItems = todos.map(todo => <li key={todo.id}>{todo.text}</li>)
```

* 如果内容的顺序会改变，那么不推荐使用序号（Index）作为 key，因为这会降低性能并且引发组件的状态问题。
* 如果你把列表项提取出来作为一个组件，那么要把 key 使用在列表组件上，而不是 `<li>` 标签上。


#### 加分回答


* key 一个元素在集合中的稳定标识，并帮助 React 识别变化。
* 如果元素的顺序可能变化，那应该避免使用序号作为 key。
* 如果你把列表项提取出来成为组件，你应该将 key 应用在组件上，而不是 `<li>` 元素上。


##### 相关链接


* [React 文档：列表和 Key](https://reactjs.org/docs/lists-and-keys.html)

</details>

<br>[⬆ 回到顶部](#内容)

### 回调引用（callback refs） 和 findDOMNode()，哪个更好？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* 更推荐使用回调引用而不是 `findDOMNode()`。


##### 相关链接


* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html#exposing-dom-refs-to-parent-components)

</details>

<br>[⬆ 回到顶部](#内容)

### What are fragments?

<details>
<summary>查看答案</summary>

Fragments allow a React component to return multiple elements without a wrapper, by grouping the children without adding extra elements to the DOM. Fragments offer better performance, lower memory usage, a cleaner DOM and can help in dealing with certain CSS mechanisms (e.g. tables, Flexbox and Grid).

```js
render() {
  return (
    <React.Fragment>
      <ChildA />
      <ChildB />
      <ChildC />
    </React.Fragment>
  );
}

// Short syntax supported by Babel 7
render() {
  return (
    <>
      <ChildA />
      <ChildB />
      <ChildC />
    </>
  );
}
```


#### 加分回答


* Fragments group multiple elements returned from a component, without adding a DOM element around them.


##### 相关链接


* [React docs on Fragments](https://reactjs.org/docs/fragments.html)

</details>

<br>[⬆ 回到顶部](#内容)

### How do you ensure methods have the correct `this` context in React component classes?

<details>
<summary>查看答案</summary>

In JavaScript classes, the methods are not bound by default. This means that their `this` context can be changed (in the case of an event handler, to the element that is listening to the event) and will not refer to the component instance. To solve this, `Function.prototype.bind()` can be used to enforce the `this` context as the component instance.

```js
constructor(props) {
  super(props);
  this.handleClick = this.handleClick.bind(this);
}

handleClick() {
  // Perform some logic
}
```

* The `bind` approach can be verbose and requires defining a `constructor`, so the new public class fields syntax is generally preferred:

```js
handleClick = () => {
  console.log('this is:', this);
}

render() {
  return (
    <button onClick={this.handleClick}>
      Click me
    </button>
  );
}
```

* You can also use an inline arrow function, because lexical `this` (referring to the component instance) is preserved:

```js
<button onClick={e => this.handleClick(e)}>Click me</button>
```

Note that extra re-rendering can occur using this technique because a new function reference is created on render, which gets passed down to child components and breaks `shouldComponentUpdate` / `PureComponent` shallow equality checks to prevent unnecessary re-renders. In cases where performance is important, it is preferred to go with `bind` in the constructor, or the public class fields syntax approach, because the function reference remains constant.


#### 加分回答


* You can either bind methods to the component instance context in the constructor, use public class fields syntax, or use inline arrow functions.


##### 相关链接


* [React docs on Handling Events](https://reactjs.org/docs/handling-events.html)
* [React docs on Passing Functions to Components](https://reactjs.org/docs/faq-functions.html#how-do-i-bind-a-function-to-a-component-instance)

</details>

<br>[⬆ 回到顶部](#内容)

### What are error boundaries in React?

<details>
<summary>查看答案</summary>

Error boundaries are React components that catch JavaScript errors anywhere in their child component tree, log those errors, and display a fallback UI instead of the component tree that crashed.

A class component becomes an error boundary if it defines a new lifecycle method called `componentDidCatch`.

```js
class ErrorBoundary extends React.Component {
  constructor(props) {
    super(props)
    this.state = { hasError: false }
  }

  componentDidCatch(error, info) {
    // Display fallback UI
    this.setState({ hasError: true })
    // You can also log the error to an error reporting service
    logErrorToMyService(error, info)
  }

  render() {
    if (this.state.hasError) {
      // You can render any custom fallback UI
      return <h1>Something went wrong.</h1>
    }
    return this.props.children
  }
}
```


#### 加分回答




##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### What are higher-order components?

<details>
<summary>查看答案</summary>

A higher-order component (HOC) is a function that takes a component as an argument and returns a new component. It is a pattern that is derived from React’s compositional nature. Higher-order components are like **pure components** because they accept any dynamically provided child component, but they won’t modify or copy any behavior from their input components.

```js
const EnhancedComponent = higherOrderComponent(WrappedComponent)
```


#### 加分回答


* They can be used for state abstraction and manipulation, props manipulation, render high jacking, etc.


##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### How to apply prop validation in React?

<details>
<summary>查看答案</summary>

When the application is running in development mode, React will automatically check for all props that we set on components to make sure they are the correct data type. For incorrect data types, it will generate warning messages in the console for development mode. They are stripped in production mode due to their performance impact. Required props are defined with `isRequired`.

For example, we define `propTypes` for component as below:

```js
import PropTypes from "prop-types"

class User extends React.Component {
  static propTypes = {
    name: PropTypes.string.isRequired,
    age: PropTypes.number.isRequired
  }

  render() {
    return (
      <h1>Welcome, {this.props.name}</h1>
      <h2>Age, {this.props.age}
    )
  }
}
```


#### 加分回答


* We can define custom `propTypes`
* Using `propTypes` is not mandatory. However, it is a good practice and can reduce bugs.


##### 相关链接



</details>

<br>[⬆ 回到顶部](#内容)

### 什么是上下文（Context）？

<details>
<summary>查看答案</summary>

上下文提供了一种通过组件树传递数据的方式，而不需要手动地在每层把参数传递下去。比如，授权的用户、语言信息、UI 主题这些需要被应用中的很多组件获取的数据。

```js
const { Provider, Consumer } = React.createContext(defaultValue)
```


#### 加分回答


* 上下文提供了一个在 React 组件树中传递数据的方式，而不需要手动地传递参数。
* 上下文被设计用来在 React 组件树中共享可以被视为*全局*的数据。


##### 相关链接


* [React 文档：上下文](https://reactjs.org/docs/context.html)

</details>

<br>[⬆ 回到顶部](#内容)

### What are refs in React? When should they be used?

<details>
<summary>查看答案</summary>

Refs provide a way to access DOM nodes or React elements created in the render method. Refs should be used sparringly, but there are some good use cases for refs, such as:

* Managing focus, text selection, or media playback.
* Triggering imperative animations.
* Integrating with third-party DOM libraries.

Refs are created using `React.createRef()` method and attached to React elements via the `ref` attribute. In order to use refs throughout the component, assign the `ref` to the instance property within the constructor:

```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props)
    this.myRef = React.createRef()
  }

  render() {
    return <div ref={this.myRef} />
  }
}
```

Refs can also be used in functional components with the help of closures.


#### 加分回答


* Refs are used to return a reference to an element.
* Refs shouldn't be overused.
* You can create a ref using `React.createRef()` and attach to elements via the `ref` attribute.


##### 相关链接


* [React docs on Refs and the DOM](https://reactjs.org/docs/refs-and-the-dom.html)

</details>

<br>[⬆ 回到顶部](#内容)

### `children` 参数是什么？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* 子元素（Children）是一个允许组件像数据一样被传递给其他组件的参数。
* React API 提供了使用这个属性的方法。


##### 相关链接


* [React docs on Children](https://reactjs.org/docs/jsx-in-depth.html#children-in-jsx)

</details>

<br>[⬆ 回到顶部](#内容)

### What are portals in React?

<details>
<summary>查看答案</summary>

Portal are the recommended way to render children into a DOM node that exists outside the DOM hierarchy of the parent component.

```js
ReactDOM.createPortal(child, container)
```

The first argument (`child`) is any renderable React child, such as an element, string, or fragment. The second argument (`container`) is a DOM element.


#### 加分回答




##### 相关链接


* [React docs on Portals](https://reactjs.org/docs/portals.html)

</details>

<br>[⬆ 回到顶部](#内容)


## HTML
### `image` 标签里面的 `alt` 属性有什么用？

<details>
<summary>查看答案</summary>

如果用户无法查看图片，`alt` 属性可以为其提供了替代的信息。除了装饰性的图片，所有的图片都应该有 `alt` 属性来描述。装饰性图片的 `alt` 属性应该留空。


#### 加分回答


* 装饰性的图片的 `alt` 属性应该留空。
* 爬虫用 `alt` 属性来理解图片内容，所以 `alt` 对于搜索引擎优化 (SEO) 是很重要的。
* 在 `alt` 属性末尾加 '.' 来改善网页可访问性(Accessibility)


##### 相关链接


* [为可访问性提供一个良好的基础](https://developer.mozilla.org/zh-CN/docs/learn/Accessibility/HTML:%E4%B8%BA%E5%8F%AF%E8%AE%BF%E9%97%AE%E6%80%A7%E6%8F%90%E4%BE%9B%E4%B8%80%E4%B8%AA%E8%89%AF%E5%A5%BD%E7%9A%84%E5%9F%BA%E7%A1%80)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the purpose of cache busting and how can you achieve it?

<details>
<summary>查看答案</summary>

Browsers have a cache to temporarily store files on websites so they don't need to be re-downloaded again when switching between pages or reloading the same page. The server is set up to send headers that tell the browser to store the file for a given amount of time. This greatly increases website speed and preserves bandwidth.

However, it can cause problems when the website has been changed by developers because the user's cache still references old files. This can either leave them with old functionality or break a website if the cached CSS and JavaScript files are referencing elements that no longer exist, have moved or have been renamed.

Cache busting is the process of forcing the browser to download the new files. This is done by naming the file something different to the old file.

A common technique to force the browser to re-download the file is to append a query string to the end of the file.

* `src="js/script.js"` => `src="js/script.js?v=2"`

The browser considers it a different file but prevents the need to change the file name.


#### 加分回答




##### 相关链接


* [Strategies for cache-busting CSS](https://css-tricks.com/strategies-for-cache-busting-css/)

</details>

<br>[⬆ 回到顶部](#内容)

### Can a web page contain multiple `<header>` elements? What about `<footer>` elements?

<details>
<summary>查看答案</summary>

Yes to both. The W3 documents state that the tags represent the header(`<header>`) and footer(`<footer>`) areas of their nearest ancestor "section". So not only can the page `<body>` contain a header and a footer, but so can every `<article>` and `<section>` element.


#### 加分回答


* W3 recommends having as many as you want, but only 1 of each for each "section" of your page, i.e. body, section etc.


##### 相关链接


* [StackOverflow Using header or footer tag twice](https://stackoverflow.com/questions/4837269/html5-using-header-or-footer-tag-twice?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa)

</details>

<br>[⬆ 回到顶部](#内容)

### Briefly describe the correct usage of the following HTML5 semantic elements: `<header>`, `<article>`,`<section>`, `<footer>`

<details>
<summary>查看答案</summary>

* `<header>` is used to contain introductory and navigational information about a section of the page. This can include the section heading, the author’s name, time and date of publication, table of contents, or other navigational information.

* `<article>` is meant to house a self-contained composition that can logically be independently recreated outside of the page without losing its meaning. Individual blog posts or news stories are good examples.

* `<section>` is a flexible container for holding content that shares a common informational theme or purpose.

* `<footer>` is used to hold information that should appear at the end of a section of content and contain additional information about the section. Author’s name, copyright information, and related links are typical examples of such content.


#### 加分回答


* Other semantic elements are `<form>` and `<table>`


##### 相关链接


* [HTML 5 Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)

</details>

<br>[⬆ 回到顶部](#内容)

### Where and why is the `rel="noopener"` attribute used?

<details>
<summary>查看答案</summary>

The `rel="noopener"` is an attribute used in `<a>` elements (hyperlinks). It prevents pages from having a `window.opener` property, which would otherwise point to the page from where the link was opened and would allow the page opened from the hyperlink to manipulate the page where the hyperlink is.


#### 加分回答


* `rel="noopener"` is applied to hyperlinks.
* `rel="noopener"` prevents opened links from manipulating the source page.


##### 相关链接


* [Open external anchors using rel="noopener"](https://developers.google.com/web/tools/lighthouse/audits/noopener)
* [About rel="noopener"](https://mathiasbynens.github.io/rel-noopener/)

</details>

<br>[⬆ 回到顶部](#内容)

### `<script>` 标签里面的 `defer` 和 `async` 属性是什么？

<details>
<summary>查看答案</summary>

如果两个属性都没写，脚本（script）会被串行地下载并执行，并且会暂停对文档（document）的解析（parsing），直到脚本执行完毕（默认行为）。脚本会按照其出现的顺序来下载并执行。

`defer` 属性在文档解析的同时下载脚本，但是会在文档解析完成之后再执行它，相当于在 `DOMContentLoaded` 事件监听器中执行脚本。所有 `defer` 的脚本会顺序执行。

`async` 属性会在文档解析的同时下载脚本，但是如果在文档解析完之前完成脚本下载，会前暂停文档解析，转而去执行脚本。`async` 的脚本执行不一定按照熟顺序。

注意：两个属性都应该用于带有 `src` 标签的 script 上（比如，非内联脚本）

```html
<script src="myscript.js"></script>
<script src="myscript.js" defer></script>
<script src="myscript.js" async></script>
```


#### 加分回答


* 在 `<head>` 里面放 `defer` 脚本，可以让浏览器在页面解析的同时下载脚本，因此相比于把脚本放在 body 末尾，这是一个更好的选择。
* 如果脚本之间有依赖，使用 `defer`。
* 如果脚本是独立的，使用 `async`。
* 如果 DOM 必须已经准备好并且脚本内容没有放在 `DOMContentLoaded` 监听器里面，使用 `defer`。


##### 相关链接


* [async vs defer attributes](http://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html)

</details>

<br>[⬆ 回到顶部](#内容)

### HTML 和 React 的事件处理有什么区别？

<details>
<summary>查看答案</summary>

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


#### 加分回答


* HTML 使用小写，React 使用驼峰。


##### 相关链接


* [React 文档：事件处理](https://reactjs.org/docs/handling-events.html)

</details>

<br>[⬆ 回到顶部](#内容)

### What are some differences that XHTML has compared to HTML?

<details>
<summary>查看答案</summary>

Some of the key differences are:

* An XHTML element must have an XHTML `<DOCTYPE>`
* Attributes values must be enclosed in quotes
* Attribute minimization is forbidden (e.g. one has to use `checked="checked"` instead of `checked`)
* Elements must always be properly nested
* Elements must always be closed
* Special characters must be escaped


#### 加分回答


* Any element can be self-closed
* Tags ands attributes are case-sensitive, usually lowercase


##### 相关链接


* [W3Schools docs for HTML and XHTML](https://www.w3schools.com/html/html_xhtml.asp)

</details>

<br>[⬆ 回到顶部](#内容)

### DOM 是什么？

<details>
<summary>查看答案</summary>

DOM（文档对象模型，Document Object Model）是一个跨平台的 API，它将 HTML 和 XML 文档视为一个节点（node）组成的树形结构。这些节点（比如元素和文本节点）是可以被程序操作的对象，并且任何可见的变化都会实时反映到文档上。在一个浏览器中，JavaScript 可以用这个 API 操作 DOM 节点，改变它们的在文档中的样式、内容和位置，或者通过事件监听器与 DOM 交互。


#### 加分回答


* DOM 被设计为独立于任何特定的编程语言，使得文档的结构可以从一个一致的 API 中获得。
* 在页面加载时，DOM 被逐渐地在浏览器中构建，这也是为什么脚本通常被放在页面的底部，或者放在 `<head>` 中并带有 `defer` 属性，或者放在一个事件监听器里面。操纵 DOM 节点的脚本应该在 DOM 构建完成之后再运行，以防止出现错误。
* `document.getElementById()` 和 `document.querySelector()` 是通常用来选择 DOM 节点的函数。
* 当一个节点的 `innerHTML` 设置为一个新值时，HTML 解析器会解析该字符串。这是一种向向节点添加动态 HTML 的简单方式。


##### 相关链接


* [MDN docs for DOM](https://developer.mozilla.org/en-US/docs/DOM)

</details>

<br>[⬆ 回到顶部](#内容)

### Discuss the differences between an HTML specification and a browser’s implementation thereof.

<details>
<summary>查看答案</summary>

HTML specifications such as `HTML5` define a set of rules that a document must adhere to in order to be “valid” according to that specification. In addition, a specification provides instructions on how a browser must interpret and render such a document.

A browser is said to “support” a specification if it handles valid documents according to the rules of the specification. As of yet, no browser supports all aspects of the `HTML5` specification (although all of the major browser support most of it), and as a result, it is necessary for the developer to confirm whether the aspect they are making use of will be supported by all of the browsers on which they hope to display their content. This is why cross-browser support continues to be a headache for developers, despite the improved specificiations.


#### 加分回答


* `HTML5` defines some rules to follow for an invalid `HTML5` document (i.e., one that contains syntactical errors)
* However, invalid documents may contain anything, so it's impossible for the specification to handle all possibilities comprehensively.
* Thus, many decisions about how to handle malformed documents are left up to the browser.


##### 相关链接


* [HTML 5.2 WWW Specifications](https://www.w3.org/TR/html52/)

</details>

<br>[⬆ 回到顶部](#内容)

### What is HTML5 Web Storage? Explain `localStorage` and `sessionStorage`.

<details>
<summary>查看答案</summary>

With HTML5, web pages can store data locally within the user’s browser.
The data is stored in name/value pairs, and a web page can only access data stored by itself.

**Differences between `localStorage` and `sessionStorage` regarding lifetime:**

* Data stored through `localStorage` is permanent: it does not expire and remains stored on the user’s computer until a web app deletes it or the user asks the browser to delete it.
* `sessionStorage` has the same lifetime as the top-level window or browser tab in which the data got stored. When the tab is permanently closed, any data stored through `sessionStorage` is deleted.

**Differences between `localStorage` and `sessionStorage` regarding storage scope:**
Both forms of storage are scoped to the document origin so that documents with different origins will never share the stored objects.

* `sessionStorage` is also scoped on a per-window basis. Two browser tabs with documents from the same origin have separate `sessionStorage` data.
* Unlike in `localStorage`, the same scripts from the same origin can't access each other's `sessionStorage` when opened in different tabs.


#### 加分回答


* Earlier, this was done with cookies.
* The storage limit is far larger (at least 5MB) than with cookies and its faster.
* The data is never transferred to the server and can only be used if the client specifically asks for it.


##### 相关链接


* [W3Schools HTML5 Webstorage](https://www.w3schools.com/html/html5_webstorage.asp)

</details>

<br>[⬆ 回到顶部](#内容)


## CSS
### 什么是 CSS BEM？

<details>
<summary>查看答案</summary>

BEM 方法是一个 CSS class 命名约定，他通过定义命名空间（namespace）来解决作用域问题，从而使 CSS 更可维护。BEM 代表着 块 元素 修饰（Block Element Modifier），其名字也是也是其结构的解释。一个**块** 是一个单独的组件，可以跨项目使用，对其子组件（元素，Elements）起到命名空间的作用。**修饰**用于当块或者元素处于一个特定的状态，或者在结构、样式上有所不同的时候。

```css
/* 块组件 */
.block {
}

/* 元素 */
.block__element {
}

/* 修饰 */
.block__element--modifier {
}
```

下面是一个有着 class 的样例：

```html
<nav class="navbar">
  <a href="/" class="navbar__link navbar__link--active"></a>
  <a href="/" class="navbar__link"></a>
  <a href="/" class="navbar__link"></a>
</nav>
```

在这种情况下，`navbar` 是块，`navbar__link` 是一个在 `navbar` 组件外没有任何意义的元素，而 `navbar__link--active` 是一个修饰，意味着 `navbar__link` 元素处于一个不同的状态。由于很啰嗦，很多人选择使用 `is-*` 作为修饰符。

```html
<a href="/" class="navbar__link is-active"></a>
```

修饰符必须被链接到元素上，而且永远不可以单独使用，否则会有作用域问题。

```css
.navbar__link.is-active {
}
```


#### 加分回答


* 作用域问题的可选的解决方案，比如 CSS-in-JS


##### 相关链接


* [编写干净、可维护的 CSS](https://hackernoon.com/writing-clean-and-maintainable-css-using-bem-methodology-1dcbf810a664)

</details>

<br>[⬆ 回到顶部](#内容)

### What are the advantages of using CSS preprocessors?

<details>
<summary>查看答案</summary>

CSS preprocessors add useful functionality that native CSS does not have, and generally make CSS neater and more maintainable by enabling DRY (Don't Repeat Yourself) principles. Their terse syntax for nested selectors cuts down on repeated code. They provide variables for consistent theming (however, CSS variables have largely replaced this functionality) and additional tools like color functions (`lighten`, `darken`, `transparentize`, etc), mixins, and loops that make CSS more like a real programming language and gives the developer more power to generate complex CSS.


#### 加分回答


* They allow us to write more maintainable and scalable CSS
* Some disadvantages of using CSS preprocessors (setup, re-compilation time can be slow etc.)


##### 相关链接


* [CSS Preprocessors](https://medium.com/@garyfagan/css-preprocessors-6f226fa16f27)

</details>

<br>[⬆ 回到顶部](#内容)

### Using flexbox, create a 3-column layout where each column takes up a `col-{n} / 12` ratio of the container.

```html
<div class="row">
  <div class="col-2"></div>
  <div class="col-7"></div>
  <div class="col-3"></div>
</div>
```

<details>
<summary>查看答案</summary>

Set the `.row` parent to `display: flex;` and use the `flex` shorthand property to give the column classes a `flex-grow` value that corresponds to its ratio value.

```css
.row {
  display: flex;
}

.col-2 {
  flex: 2;
}

.col-7 {
  flex: 7;
}

.col-3 {
  flex: 3;
}
```


#### 加分回答




##### 相关链接


* [MDN docs for basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
* [A complete guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

</details>

<br>[⬆ 回到顶部](#内容)

### Can you name the four types of `@media` properties?

<details>
<summary>查看答案</summary>

* `all`, which applies to all media type devices
* `print`, which only applies to printers
* `screen`, which only applies to screens (desktops, tablets, mobile etc.)
* `speech`, which only applies to screenreaders


#### 加分回答




##### 相关链接


* [MDN docs for `@media` rule](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)
* [MDN docs for using media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)

</details>

<br>[⬆ 回到顶部](#内容)

### Describe the layout of the CSS Box Model and briefly describe each component.

<details>
<summary>查看答案</summary>

<!-- Your answer goes here. -->

`Content`: The inner-most part of the box filled with content, such as text, an image, or video player. It has the dimensions `content-box width` and `content-box height`.

`Padding`: The transparent area surrounding the content. It has dimensions `padding-box width` and `padding-box height`.

`Border`: The area surrounding the padding (if any) and content. It has dimensions `border-box width` and `border-box height`.

_Margin_: The transparent outer-most layer that surrounds the border. It separates the element from other elements in the DOM. It has dimensions `margin-box width` and `margin-box height`.

![alt text](https://www.washington.edu/accesscomputing/webd2/student/unit3/images/boxmodel.gif)


#### 加分回答


* This is a very common question asked during front-end interviews and while it may seem easy, it is critical you know it well!
* Shows a solid understanding of spacing and the DOM


##### 相关链接


* [W3School's CSS Box Model Page](https://www.w3schools.com/Css/css_boxmodel.asp)
* [Mozilla's Intro to the CSS Box Model](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the difference between `em` and `rem` units?

<details>
<summary>查看答案</summary>

Both `em` and `rem` units are based on the `font-size` CSS property. The only difference is where they inherit their values from.

* `em` units inherit their value from the `font-size` of the parent element
* `rem` units inherit their value from the `font-size` of the root element (`html`)

In most browsers, the `font-size` of the root element is set to `16px` by default.


#### 加分回答


* Benefits of using `em` and `rem` units


##### 相关链接


* [CSS units for font-size: px | em | rem](https://medium.com/code-better/css-units-for-font-size-px-em-rem-79f7e592bb97)

</details>

<br>[⬆ 回到顶部](#内容)

### What are the advantages of using CSS sprites and how are they utilized?

<details>
<summary>查看答案</summary>

CSS sprites combine multiple images into one image, limiting the number of HTTP requests a browser has to make, thus improving load times. Even under the new HTTP/2 protocol, this remains true.

Under HTTP/1.1, at most one request is allowed per TCP connection. With HTTP/1.1, modern browsers open multiple parallel connections (between 2 to 8) but it is limited. With HTTP/2, all requests between the browser and the server are multiplexed on a single TCP connection. This means the cost of opening and closing multiple connections is mitigated, resulting in a better usage of the TCP connection and limits the impact of latency between the client and server. It could then become possible to load tens of images in parallel on the same TCP connection.

However, according to [benchmark results](https://blog.octo.com/en/http2-arrives-but-sprite-sets-aint-no-dead/), although HTTP/2 offers 50% improvement over HTTP/1.1, in most cases the sprite set is still faster to load than individual images.

To utilize a spritesheet in CSS, one would use certain properties, such as `background-image`, `background-position` and `background-size` to ultimately alter the `background` of an element.


#### 加分回答


* `background-image`, `background-position` and `background-size` can be used to utilize a spritesheet.


##### 相关链接


* [CSS Sprites explained by CSS Tricks](https://css-tricks.com/css-sprites/)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the difference between '+' and '~' sibling selectors?.

<details>
<summary>查看答案</summary>

The General Sibling Selector `~` selects all elements that are siblings of a specified element.

The following example selects all `<p>` elements that are siblings of `<div>` elements:

```css
div ~ p {
  background-color: blue;
}
```

The Adjacent Sibling Selector `+` selects all elements that are the adjacent siblings of a specified element.

The following example will select all `<p>` elements that are placed immediately after `<div>` elements:

```css
div + p {
  background-color: red;
}
```


#### 加分回答




##### 相关链接


* [W3School's CSS Combinators Page](https://www.w3schools.com/css/css_combinators.asp)
* [Mozilla's Combinators and groups of selectors page](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors)

</details>

<br>[⬆ 回到顶部](#内容)

### Can you describe how CSS specificity works?

<details>
<summary>查看答案</summary>

Assuming the browser has already determined the set of rules for an element, each rule is assigned a matrix of values, which correspond to the following from highest to lowest specificity:

* Inline rules (binary - 1 or 0)
* Number of id selectors
* Number of class, pseudo-class and attribute selectors
* Number of tags and pseudo-element selectors

When two selectors are compared, the comparison is made on a per-column basis (e.g. an id selector will always be higher than any amount of class selectors, as ids have higher specificity than classes). In cases of equal specificity between multiple rules, the rules that comes last in the page's style sheet is deemed more specific and therefore applied to the element.


#### 加分回答


* Specificity matrix: [inline, id, class/pseudo-class/attribute, tag/pseudo-element]
* In cases of equal specificity, last rule is applied


##### 相关链接


* [CSS Specificity](https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/)

</details>

<br>[⬆ 回到顶部](#内容)

### What is a focus ring? What is the correct solution to handle them?

<details>
<summary>查看答案</summary>

A focus ring is a visible outline given to focusable elements such as buttons and anchor tags. It varies depending on the vendor, but generally it appears as a blue outline around the element to indicate it is currently focused.

In the past, many people specified `outline: 0;` on the element to remove the focus ring. However, this causes accessibility issues for keyboard users because the focus state may not be clear. When not specified though, it causes an unappealing blue ring to appear around an element.

In recent times, frameworks like Bootstrap have opted to use a more appealing `box-shadow` outline to replace the default focus ring. However, this is still not ideal for mouse users.

The best solution is an upcoming pseudo-selector `:focus-visible` which can be polyfilled today with JavaScript. It will only show a focus ring if the user is using a keyboard and leave it hidden for mouse users. This keeps both aesthetics for mouse use and accessibility for keyboard use.


#### 加分回答




##### 相关链接


* [:focus-visible](https://css-tricks.com/focus-visible-and-backwards-compatibility/)

</details>

<br>[⬆ 回到顶部](#内容)


## Node
### NodeJS often uses a callback pattern where if an error is encountered during execution, this error is passed as the first argument to the callback. What are the advantages of this pattern?

```js
fs.readFile(filePath, function(err, data) {
  if (err) {
    // handle the error, the return is important here
    // so execution stops here
    return console.log(err)
  }
  // use the data object
  console.log(data)
})
```

<details>
<summary>查看答案</summary>

Advantages include:

* Not needing to process data if there is no need to even reference it
* Having a consistent API leads to more adoption
* Ability to easily adapt a callback pattern that will lead to more maintainable code

As you can see from below example, the callback is called with null as its first argument if there is no error. However, if there is an error, you create an Error object, which then becomes the callback's only parameter. The callback function allows a user to easily know whether or not an error occurred.

This practice is also called the _Node.js error convention_, and this kind of callback implementations are called _error-first callbacks_.

```js
var isTrue = function(value, callback) {
  if (value === true) {
    callback(null, "Value was true.")
  } else {
    callback(new Error("Value is not true!"))
  }
}

var callback = function(error, retval) {
  if (error) {
    console.log(error)
    return
  }
  console.log(retval)
}

isTrue(false, callback)
isTrue(true, callback)

/*
  { stack: [Getter/Setter],
    arguments: undefined,
    type: undefined,
    message: 'Value is not true!' }
  Value was true.
*/
```


#### 加分回答


* This is just a convention. However, you should stick to it.


##### 相关链接


* [The Node.js Way Understanding Error-First Callbacks](http://fredkschott.com/post/2014/03/understanding-error-first-callbacks-in-node-js/)
* [What are the error conventions?](https://docs.nodejitsu.com/articles/errors/what-are-the-error-conventions)

</details>

<br>[⬆ 回到顶部](#内容)

### What is REST?

<details>
<summary>查看答案</summary>

REST (REpresentational State Transfer) is a software design pattern for network architecture. A RESTful web application exposes data in the form of information about its resources.

Generally, this concept is used in web applications to manage state. With most applications, there is a common theme of reading, creating, updating, and destroying data. Data is modularized into separate tables like `posts`, `users`, `comments`, and a RESTful API exposes access to this data with:

* An identifier for the resource. This is known as the endpoint or URL for the resource.
* The operation the server should perform on that resource in the form of an HTTP method or verb. The common HTTP methods are GET, POST, PUT, and DELETE.

Here is an example of the URL and HTTP method with a `posts` resource:

* Reading: `/posts/` => GET
* Creating: `/posts/new` => POST
* Updating: `/posts/:id` => PUT
* Destroying: `/posts/:id` => DELETE


#### 加分回答


* Alternatives to this pattern like GraphQL


##### 相关链接


*   ](https://medium.com/extend/what-is-rest-a-simple-explanation-for-beginners-part-1-introduction-b4a072f8740f)

</details>

<br>[⬆ 回到顶部](#内容)

### 如何避免回调地狱？

```js
getData(function(a) {
  getMoreData(a, function(b) {
    getMoreData(b, function(c) {
      getMoreData(c, function(d) {
        getMoreData(d, function(e) {
          // ...
        })
      })
    })
  })
})
```

<details>
<summary>查看答案</summary>

一般最好的方式是用 `async/await` 将函数重构，使其返回一个 promise。相比较于给函数传递一个回调而造成深层的嵌套，这种方式可以返回一个可以用于 `await` 的 promise，并且可以在数据一返回就被处理，而下一行代码也可以以一种类似同步（sync-like）的方式执行。

上面的代码可以被重构如下：

```js
async function asyncAwaitVersion() {
  const a = await getData()
  const b = await getMoreData(a)
  const c = await getMoreData(b)
  const d = await getMoreData(c)
  const e = await getMoreData(d)
  // ...
}
```

有很多可以解决回调地狱的方法：

* 模块化（Modularization）：将回调拆分成独立的函数。
* 使用一个流程控制库，比如 async。
* 搭配 generator 使用 promise。
* 使用 async/await （node v7 以上）。


#### 加分回答


* 作为一个高效的 JavaScript 开发者，你必须要避免不断增长的缩进级别，要书写干净且可读的代码，并且可以处理复杂的流程。


##### 相关链接


* [避免 Node.js 中的回调地狱](http://stackabuse.com/avoiding-callback-hell-in-node-js/)
* [异步 JavaScript：从 Callback 到 Async、Await](https://blog.hellojs.org/asynchronous-javascript-from-callback-hell-to-async-and-await-9b9ceb63c8e8)

</details>

<br>[⬆ 回到顶部](#内容)

### What is the event loop in Node.js?

<details>
<summary>查看答案</summary>

The event loop handles all async callbacks. Callbacks are queued in a loop, while other code runs, and will run one by one when the response for each one has been received.


#### 加分回答


* The event loop allows Node.js to perform non-blocking I/O operations, despite the fact that JavaScript is single-threaded


##### 相关链接


* [Node.js docs on event loop, timers and process.nextTick()](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)

</details>

<br>[⬆ 回到顶部](#内容)


## Security
### What is a cross-site scripting attack (XSS) and how do you prevent it?

<details>
<summary>查看答案</summary>

XSS refers to client-side code injection where the attacker injects malicious scripts into a legitimate website or web application. This is often achieved when the application does not validate user input and freely injects dynamic HTML content.

For example, a comment system will be at risk if it does not validate or escape user input. If the comment contains unescaped HTML, the comment can inject a `<script>` tag into the website that other users will execute against their knowledge.

* The malicious script has access to cookies which are often used to store session tokens. If an attacker can obtain a user’s session cookie, they can impersonate the user.
* The script can arbitrarily manipulate the DOM of the page the script is executing in, allowing the attacker to insert pieces of content that appear to be a real part of the website.
* The script can use AJAX to send HTTP requests with arbitrary content to arbitrary destinations.


#### 加分回答


* On the client, using `textContent` instead of `innerHTML` prevents the browser from running the string through the HTML parser which would execute scripts in it.
* On the server, escaping HTML tags will prevent the browser from parsing the user input as actual HTML and therefore won't execute the script.


##### 相关链接


* [Cross-Site Scripting Attack (XSS)](https://www.acunetix.com/websitesecurity/cross-site-scripting/)

</details>

<br>[⬆ 回到顶部](#内容)


## License

[MIT](LICENSE). Copyright (c) [Stefan Feješ](https://stefanfejes.com/).
