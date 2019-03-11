### 创建一个独立的 `bind` 函数，其功能等价于 `Function.prototype.bind` 。

```js
function example() {
  console.log(this)
}
const boundExample = bind(example, { a: true })
boundExample.call({ b: true }) // logs { a: true }
```

#### Answer

返回一个函数，该函数接受任意数量的参数，并将它们用剩余参数运算符 `...` 收集起来。该函数使用 `fn` 调用 `Function.prototype.apply` 并传入上下文（context）和传入的参数数组，最后将结果返回。

```js
const bind = (fn, context) => (...args) => fn.apply(context, args)
```

#### Good to hear

##### Additional links

<!-- Whenever possible, link a more detailed explanation. -->

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
