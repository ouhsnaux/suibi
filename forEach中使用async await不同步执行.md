# forEach中使用async await不同步执行

是的，不会同步执行，`forEach` 不会判断第一个参数是不是promise，以及特殊处理。

解决方法也比较简单，改成 `for` `while` 或 `for...of`。
`for...of` 拿不到 `index`，可以使用 `for(const [index, item] of list.entries())`。
