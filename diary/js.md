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