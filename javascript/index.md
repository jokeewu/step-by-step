# JavaScript重要知识点

### **严格模式**

### **数据类型**

number string boolean undefined null object symbol

### **实现继承方式**

#### **原型继承**
#### **构造函数继承**
#### **组合继承（原型+构造函数）**

### **func.bind(obj1).bind(obj2).bind(obj3)**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Function/bind](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Function/bind)

### **e.target,e.currentTarget分别指的什么?**

### **闭包、this**

### **函数截流、防抖**

参见：[https://segmentfault.com/a/1190000002764479](https://segmentfault.com/a/1190000002764479)

### **函数柯里化**

### **箭头函数，this指向**

词法作用域，由其上下文决定，参见：[https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions/arrow_functions](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions/arrow_functions)
  - apply/call/bind无法修改this指向
  - 不绑定arguments
  - 箭头函数不能作为构造函数，和new一起使用会报错
  - 箭头函数没有prototype属性
  - yield关键字不能在箭头函数中使用
  - 箭头函数具有与常规函数不同的特殊运算符优先级解析规则

### **DOM事件**

阶段：捕获、目标、冒泡

事件委托

级别：DOM0、DOM2、DOM3

### **script标签async、defer属性**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/script](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/script)

### **Event Loop、微任务、宏任务**

参见：[https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/EventLoop](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/EventLoop)

### **toString、valueOf区别**

参见：

原始值：https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Data_structures

https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/toString

https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/valueOf

### **===/==**

https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/Comparison_Operators

### **new Object()做了哪些操作?**

https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/new

### **Promise.reslove(1).then().then()**

### **对象深拷贝**

JSON.stringify

递归，循环引用，不同数据类型

### **async、await, iterator、generator**

http://www.ruanyifeng.com/blog/2015/05/async.html
http://www.ruanyifeng.com/blog/2015/04/generator.html

### **for...of与for…in区别**

for…of对象必须包含Symbol.iterator属性，不能遍历普通对象
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol/iterator

## **标记模版字面量如何使用？**

## **null/undefined区别
