### `0.1 + 0.2 === 0.3` 的值是什么？

#### Answer

它的计算结果是 `false`，因为 JavaScript 的数学计算使用 IEEE 754 标准，并且使用了 64 位的浮点数。这造成了在进行小数运算时的精度问题，简而言之，这是因为计算机是基于二进制工作的，而小数是十进制的。

```js
0.1 + 0.2 // 0.30000000000000004
```

可以通过一个函数来判断两个数字是否大致相等来解决该问题。该函数定义一个误差值（Error margin），判断两个值的差值是否小于该误差值。

```js
const approxEqual = (n1, n2, epsilon = 0.0001) => Math.abs(n1 - n2) < epsilon
approxEqual(0.1 + 0.2, 0.3) // true
```

#### Good to hear

* 解决该问题的简单方法

##### Additional links

* [一个检测相等性的简单辅助函数](https://github.com/Chalarangelo/30-seconds-of-code#approximatelyequal)
* [解决 JavaScript 中的 "0.1 + 0.2 = 0.300000004"](http://blog.blakesimpson.co.uk/read/61-fix-0-1-0-2-0-300000004-in-javascript)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
