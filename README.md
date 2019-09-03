# 前言
JavaScript知识点梳理

[1.请写出如下代码的打印结果](https://github.com/fuhangyy/Vue-Blog/issues/1)
```js
function Foo() {
  Foo.a = function () {
    console.log(1)
  }
  this.a = function () {
    console.log(2)
  }
}
Foo.prototype.a = function () {
  console.log(3)
}
Foo.a = function () {
  console.log(4)
}
Foo.a();
let obj = new Foo();
obj.a();
Foo.a();
```
