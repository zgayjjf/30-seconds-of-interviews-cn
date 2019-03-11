### 什么是大 O 符号？

#### Answer

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

#### Good to hear

* 当执行时间呈指数增长时，要小心嵌套循环。

##### Additional links

<!-- Whenever possible, link a more detailed explanation. -->

* [JavaScript 的大 O 符号](https://medium.com/cesars-tech-insights/big-o-notation-javascript-25c79f50b19b)

<!-- tags: (javascript) -->

<!-- expertise: (2) -->
