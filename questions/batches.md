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

#### Answer

我们必须有所有的配方中可用的原材料，而且数量要大于或等于所需的材料数量。只要有一个原材料不可用或低于我们需要的，我们就无法做哪怕一批。

用 `Object.keys()` 获得原材料的数组，再用 `Array.prototype.map()` 将每一个原材料映射到可用原材料的数量与配饭所需数量的比例。如果一个配方所需的原材料不可用，该比例会被计算为 `NaN`，所以或逻辑运算符 `||` 可以用于将这种情况回退到 `0`。

用扩展运算符 `...` ，将原材料数组传入 `Math.min()` 来找到最小的比例。将最后的结果传入 `Math.floor()`，从而将结果舍尾成可做的最大数量。

```js
const batches = (recipe, available) =>
  Math.floor(
    Math.min(...Object.keys(recipe).map(k => available[k] / recipe[k] || 0))
  )
```

#### Good to hear

##### Additional links

<!-- Whenever possible, link a more detailed explanation. -->

<!-- tags: (javascript) -->

<!-- expertise: (1) -->
