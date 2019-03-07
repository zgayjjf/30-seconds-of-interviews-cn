### 什么是 CSS BEM？

#### Answer

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

在这种情况下，`navbar` 是块，`navbar__link` 是一个在 `navbar` 组件外没有任何意义的元素，而 `navbar__link--active` 是一个修饰，意味着 `navbar__link` 元素处于一个不同的状态。
由于秀使其很啰嗦，很多人选择使用 `is-*` 作为修饰符。

```html
<a href="/" class="navbar__link is-active"></a>
```

修饰符必须被链接到元素上，而且永远不可以单独使用，否则会有作用域问题。

```css
.navbar__link.is-active {
}
```

#### Good to hear

* 作用域问题的可选的解决方案，比如 CSS-in-JS

##### Additional links

* [编写干净、可维护的CSS](https://hackernoon.com/writing-clean-and-maintainable-css-using-bem-methodology-1dcbf810a664)

<!-- tags: (css) -->

<!-- expertise: (0) -->
