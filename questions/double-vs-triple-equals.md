### 相等操作符 `==` 和 `===` 的区别是什么？

#### Answer

三等号 (`===`) 检查是否严格相等，意即：类型和值都要一样。双等号则会首先进行强制类型转换，使得等号两边对象拥有同样的类型，再进行严格的比较。

#### Good to hear

* 尽可能使用三等号来做相等比较，因为宽松相等 `==` 会有反直觉的结果。
* 强制类型转换意味着所有的值都会被转化为同样的类型。
* 提到假值 (Falsy values) 和他们的比较。

##### Additional links

* [MDN 比较操作符](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators)

<!-- tags: (javascript) -->

<!-- expertise: (0) -->

#### 译者注

`===` 一般翻译为**一致(Identity)**、**严格相等(Strict Equality)**、**三等号(Triple Equals)**；`==` 一般翻译为**相等（Equal）**、**一般相等/宽松相等(Loose Equality)、抽象相等(Abstract Equality )、双等号(Double Equals)**
