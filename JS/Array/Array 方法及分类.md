# Array 方法分类

数组方法非常多，在JS编程中使用非常频繁，对数组方法分类便于理解和加深记忆。

## 改变原数组

> [push (element1, ..., elementN)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/push)<br>
> 将一个或多个元素 `添加` 到数组的 `末尾`，并返回该数组的 `新长度`<br><br>
> [unshift (element1, ..., elementN)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift)<br>
> 将一个或多个元素 `添加` 到数组的`开头`，并返回该数组的`新长度`<br><br>
> [pop ( )](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/pop)<br>
> `删除` `最后` 一个元素，并返回 `该元素的值`<br><br>
> [shift ( )](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/shift)<br>
> `删除` `第一个` 元素，并返回 `该元素的值`<br><br>
> [splice (start[, deleteCount[, item1[, item2[, ...]]]])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)<br>
> `删除` 指定 `位置` 开始指定 `长度` 的元素，并 `添加` 零个或多个元素，返回 `被删除的项`<br><br>
> [reverse ( )](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)<br>
> 将数组中元素的位置 `颠倒`，并返回 `该数组`<br><br>
> [sort ([compareFunction])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)<br>
> 对数组的元素进行 `排序`，并返回 `该数组`

## 不改变原数组

> [slice ([begin[, end]])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/slice)<br>
> `提取` 原数组元素，由 begin 和 end 决定的原数组的浅拷贝（包括 begin，不包括end）<br><br>
> [concat (value1[, value2[, ...[, valueN]]])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/concat)<br>
> `合并` 两个或多个数组<br><br>
> [join ([separator])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/join)<br>
> 所有元素 `连接` 成一个字符串并返回这个字符串<br><br>
> [toString ( )](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/toString)<br>
> 返回字符串等同于 `join()`<br><br>
> [indexOf (searchElement[, fromIndex)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf)<br>
> 在数组中可以找到一个给定元素的 `第一个索引`，如果不存在，则返回-1<br><br>
> [lastIndexOf (searchElement[, fromIndex])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/lastIndexOf)<br>
> 在数组中的 `最后一个的索引`，如果不存在则返回 -1。从数组的后面向前查找，从 fromIndex 处开始<br><br>
> [copyWithin (target[, start[, end]])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/copyWithin)<br>
> 浅复制数组的一部分到同一数组中的另一个位置

## 操作Array元素的callback的方法集合

> [every (callback[, thisArg])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/every)<br>
> 测试一个数组内的所有元素是否 `都能通过` 某个指定函数的测试。它返回一个布尔值。<br><br>

## 返回Array 迭代器对象

> [entries (target[, start[, end]])](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/copyWithin)<br>
> 返回一个新的 `Array Iterator` 对象，该对象包含数组中每个索引的键/值对<br><br>
