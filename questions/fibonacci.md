### 生成一个包含 n 项斐波那契数列的数组。

#### Answer

初始化一个长度为 n 的空数组。使用 `Array.prototype.reduce()` 在数组中增加值，每个值都是前面最后两个值的和（除了最开始两个值）。

```js
const fibonacci = n =>
  [...Array(n)].reduce(
    (acc, val, i) => acc.concat(i > 1 ? acc[i - 1] + acc[i - 2] : i),
    []
  )
```

#### Good to hear

##### Additional links

* [类似问题](https://github.com/Chalarangelo/30-seconds-of-code/blob/master/snippets_archive/fibonacciUntilNum.md)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
