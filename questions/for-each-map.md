### 数组方法 `map()` 和 `forEach()` 的区别是什么？

#### Answer

两个方法都会变量数组的所有元素。`map()` 通过在每个元素上调用回调函数，从而将每个元素映射为一个新的元素，并返回一个新的数组。另一方面，`forEach()` 为每个元素调用回调函数，但是不返回一个新的数组。`forEach()` 通常被用于引发副作用的迭代，而 `map()` 通常用于函数式编程

#### Good to hear

* `forEach()` 用于以下场景：如果你需要对一个数组进行迭代，并且改变元素，同时不需要生成一个新的数组。
* `map()` 用于需要保持数据不可变的情况，此时所有的原数组中的数据都会被映射到一个新的数组中。

##### Additional links

* [MDN docs for forEach](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
* [MDN docs for map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
* [JavaScript — Map vs. ForEach](https://codeburst.io/javascript-map-vs-foreach-f38111822c0f)

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
