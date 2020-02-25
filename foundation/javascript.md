# JavaScript重要知识点

## **语言本身**

### **严格模式**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Strict_mode](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Strict_mode)

### **数据类型/原始值**

原始值类型：Number、BigInt、String、Boolean、Undefined、Null、Symbol

引用类型：Object

null是原始值，为什么`typeof null === 'object'`？参见：
- [https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/typeof#null](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/typeof#null)
- [https://2ality.com/2013/10/typeof-null.html](https://2ality.com/2013/10/typeof-null.html)

### **实现继承方式**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Inheritance_and_the_prototype_chain](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)

#### **原型继承**
#### **构造函数继承**
#### **组合继承（原型+构造函数）**

### **func.bind(obj1).bind(obj2).bind(obj3)**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Function/bind](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Function/bind)

### **闭包、this**

### **函数柯里化**

### **箭头函数，this指向**

词法作用域，由其上下文决定，参见：[https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions/arrow_functions](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions/arrow_functions)

  - apply/call/bind无法修改this指向
  - 不绑定arguments
  - 箭头函数不能作为构造函数，和new一起使用会报错
  - 箭头函数没有prototype属性
  - yield关键字不能在箭头函数中使用
  - 箭头函数具有与常规函数不同的特殊运算符优先级解析规则

### **toString、valueOf区别**

参见：

原始值：
- https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Data_structures
- https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/toString
- https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/valueOf

### **===/==，相等判断**

参见：
- [https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Equality_comparisons_and_sameness](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Equality_comparisons_and_sameness)
- [https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/Comparison_Operators](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/Comparison_Operators)

### **Promise.reslove(1).then().then()**

### **async、await, iterator、generator**

http://www.ruanyifeng.com/blog/2015/05/async.html
http://www.ruanyifeng.com/blog/2015/04/generator.html

### **for...of与for…in区别**

for…of对象必须包含Symbol.iterator属性，不能遍历普通对象
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol/iterator

### **标记模版字面量如何使用？**

### **null/undefined区别**

undefined
* 一个声明未定义的变量的初始值，或没有实际参数的形式参数
* undefined作为全局对象的一个属性

null
* 表示缺少的标识，特指对象的值未设置

参见：
- [https://developer.mozilla.org/en-US/docs/Glossary/undefined](https://developer.mozilla.org/en-US/docs/Glossary/undefined)
- [https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/undefined](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/undefined)
- [https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/null](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/null)
- []()

### **Common JS/Import区别**

### **export/export default区别**

---
---

## **宿主环境**

### **e.target,e.currentTarget分别指的什么？**

### **DOM事件**

阶段：捕获、目标、冒泡

事件委托

级别：DOM0、DOM2、DOM3

### **script标签async、defer属性**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/script](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/script)

### **Event Loop、微任务、宏任务**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/EventLoop](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/EventLoop)

### **Ajax/Fetch，fetch有哪些优势？**

参见：[https://www.cnblogs.com/chris-oil/p/6014323.html](https://www.cnblogs.com/chris-oil/p/6014323.html)

### **setTimeout(f, 0)使用场景**

### **Cookie，session，localStorage，sessionStorage，后端怎么存储session?**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Cookies](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Cookies)

### **跨域解决方案**

jsonp，proxy，header(Access-Control-Allow-Origin)，domain，name，postMessage