### JavaScript 中的真值（Truthy）和假值（Falsy）是什么？

#### Answer

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

#### Good to hear

##### Additional links

* [Truthy on MDN](https://developer.mozilla.org/en/docs/Glossary/Truthy)
* [Falsy on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)

<!-- Whenever possible, link a more detailed explanation. -->

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
