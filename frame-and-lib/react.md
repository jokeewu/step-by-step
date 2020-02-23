# React 重要知识点

### **生命周期**

参见：[https://reactjs.org/docs/react-component.html](https://reactjs.org/docs/react-component.html)

### **componentWillReceiveProps取消原因**

参见：[https://reactjs.org/docs/react-component.html](https://reactjs.org/docs/react-component.html)

### **This.setState() 触发了哪些生命周期函数？什么情况下会同步执行？**

### **Render props/HOC比较**

HOC作用：属性代理，反向继承

设计模式：装饰模式

反向继承

```javascript
func hoc() {
    class extends SuperComponent {
        // ...
        render() {
            return super.render()
        }
    }
}
```

### **element、Component、Node区别是什么？**

### **key的作用**

参见：[https://reactjs.org/docs/lists-and-keys.html](https://reactjs.org/docs/lists-and-keys.html)

### **Fiber、diff算法**

参见：[https://reactjs.org/docs/reconciliation.html](https://reactjs.org/docs/reconciliation.html)

### **Context作用**

参见：[https://reactjs.org/docs/context.html](https://reactjs.org/docs/context.html)

### **React.memo、Hooks等**

---

## 性能优化