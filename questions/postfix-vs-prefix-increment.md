### 后缀自增运算符 `i++` 和 前缀自增运算符 `++i` 有什么区别？

#### Answer

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

#### Good to hear

##### Additional links

<!-- tags: (javascript) -->

<!-- expertise: (0) -->
