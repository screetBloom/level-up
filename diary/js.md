### js中指针问题
根据js本身的一些特性，在具体编程的时候，利用这些特性来让代码更加的简洁、明了

#### 函数参数传递问题
```js
function test(person) {
  person.age = 26
  person = {
    name: 'hzj',
    age: 18
  }
  return person
}
const p1 = {
  name: 'fyq',
  age: 19
}
const p2 = test(p1)
console.log(p1); // {name: “fyq”, age: 26}
console.log(p2); // p2：{name: “hzj”, age: 18}
```

**解释：**
- 在函数传参的时候传递的是对象在堆中的内存地址值
    - test函数中的实参person是p1对象的内存地址，通过调用person.age = 26确实改变了p1的值
- 随后person变成了另一块内存空间的地址
    - 在最后将这另外一份内存空间的地址返回，赋给了p2。
    
### js类型转换问题
js自身的实现，决定了它在进行类型转换时的求原始值调用顺序

#### ==和===转换规则
==不像===那样严格，对于一般情况，只要值相等，就返回true，但==还涉及一些类型转换，它的转换规则如下：

- 两边的类型是否相同，相同的话就比较值的大小，例如1==2，返回false
- 判断的是否是null和undefined，是的话就返回true
- 判断的类型是否是String和Number，是的话，把String类型转换成Number，再进行比较
- 判断其中一方是否是Boolean，是的话就把Boolean转换成Number，再进行比较
- 如果其中一方为Object，且另一方为String、Number或者Symbol，会将Object转换成字符串，再进行比较

```js
console.log({a: 1} == true);//false
console.log({a: 1} == "[object Object]");//true
```

#### 对象转原始值
对象转原始类型，会调用内置的[ToPrimitive]函数，对于该函数而言，其逻辑如下：

如果Symbol.toPrimitive()方法，优先调用再返回
调用valueOf()，如果转换为原始类型，则返回
调用toString()，如果转换为原始类型，则返回
如果都没有返回原始类型，会报错
```js
var obj = {
  value: 3,
  valueOf() {
    return 4;
  },
  toString() {
    return '5'
  },
  [Symbol.toPrimitive]() {
    return 6
  }
}
console.log(obj + 1); // 输出7
```

**引申：** 如何让if(a == 1 && a == 2)条件成立？<br>
```js
var a = {
  value: 0,
  valueOf() {
    return ++this.value;
  }
};
console.log(a == 1 && a == 2); //true
```