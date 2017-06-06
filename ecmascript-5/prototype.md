在 JavaScript 中，函数是一个包含属性和方法的 Function 类型的对象。而原型（Prototype）就是 Function 类型对象的一个属性。


function foo(a,b){
```

## 获取原型

function Person() {
```

- 通过 Object 对象的 getPrototypeOf( obj ) 方法。

```javascript
function Person() {
```

## 原型的属性和方法

- 原型的属性和方法单独进行定义。
构造函数.prototype.属性名 = 属性值;
```

- 直接为原型定义一个新对象。
构造函数.prototype = {
```

## 自有属性与原型属性

```javascript
function Emp( ename, salary ){
```

上述代码的内存结构图如下:

![](19.png)

## 检测自有或原型属性

```javascript
function Hero(){}
```

- 使用 in 关键字检测对象及其原型链中是否具有指定属性:

```javascript
function Hero(){}
```

## 扩展属性或方法

```javascript
functon Hero(){}
```

## 重写原型属性

```javascript
functon Hero(){}
```

## 删除属性

```javascript
functon Hero(){}
```

## isPrototypeOf() 方法

每个对象中都会具有一个 isPrototypeOf() 方法，该方法用来判断一个对象是否是另一个对象的原型。
var monkey = {}
```

## `__proto__` 属性
functon Hero(){}
```

上述代码说明 hero 对象存在一个指向构造函数 Hero 的原型，这个链接被叫做 `__proto__` 属性。

> **值得注意的是:** `__proto__` 属性与 prototype 属性并不等价。
> 
> - `__proto__` 属性是指定对象的属性。
> - prototype 属性是指定构造函数的属性。
> 
> 再有就是，`__proto__` 属性只能在学习或调试的时候使用。

## 扩展内建对象



如下代码示例，利用 Array 对象的 prototype 属性扩展了 inArray() 方法。
Array.prototype.inArray = function(color){
```