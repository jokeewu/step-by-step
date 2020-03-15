## React 重要知识点

[React哲学](https://zh-hans.reactjs.org/docs/thinking-in-react.html)

### **生命周期**

挂载阶段(Mounting)：
- constructor()
- static getDerivedStateFromProps()
- render()
- componentDidMount()

更新阶段(Updating)：
- static getDerivedStateFromProps()
- shouldComponentUpdate()
- render()
- getSnapshotBeforeUpdate()
- componentDidUpdate()

卸载阶段(Unmounting)：
- componentWillUnmount()

错误处理(Error Handling)：
- static getDerivedStateFromError()
- componentDidCatch()

参见：[https://reactjs.org/docs/react-component.html](https://reactjs.org/docs/react-component.html)

### **componentWillReceiveProps取消原因**

参见：[https://reactjs.org/docs/react-component.html](https://reactjs.org/docs/react-component.html)

### **`this.setState()` 触发了哪些生命周期函数？什么情况下会同步执行？**

- [https://zh-hans.reactjs.org/docs/react-component.html#setstate](https://zh-hans.reactjs.org/docs/react-component.html#setstate)

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

参考:

- [https://zh-hans.reactjs.org/docs/higher-order-components.html](https://zh-hans.reactjs.org/docs/higher-order-components.html)
- [https://zh-hans.reactjs.org/docs/render-props.html](https://zh-hans.reactjs.org/docs/render-props.html)

### **element、Component、Node区别是什么？**

参见：
- [https://zh-hans.reactjs.org/docs/rendering-elements.html](https://zh-hans.reactjs.org/docs/rendering-elements.html)

### **key的作用**

参见：[https://reactjs.org/docs/lists-and-keys.html](https://reactjs.org/docs/lists-and-keys.html)

### **Fiber、diff算法**

参见：[https://reactjs.org/docs/reconciliation.html](https://reactjs.org/docs/reconciliation.html)

### **Context作用**

参见：[https://reactjs.org/docs/context.html](https://reactjs.org/docs/context.html)

### **React.memo、Hooks等**

- [hooks使用原则](https://zh-hans.reactjs.org/docs/hooks-rules.html)

## 性能优化

- [https://zh-hans.reactjs.org/docs/optimizing-performance.html](https://zh-hans.reactjs.org/docs/optimizing-performance.html)
- [https://zh-hans.reactjs.org/docs/profiler.html](https://zh-hans.reactjs.org/docs/profiler.html)

---

## **VUE知识点**

### **生命周期**

参见：[https://cn.vuejs.org/v2/guide/instance.html#%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F%E5%9B%BE%E7%A4%BA](https://cn.vuejs.org/v2/guide/instance.html#%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F%E5%9B%BE%E7%A4%BA)

### **响应式系统原理**

参见：
- [https://cn.vuejs.org/v2/guide/reactivity.html](https://cn.vuejs.org/v2/guide/reactivity.html)
- [https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty)

### **动态组件/异步组件**

参见：
- [https://cn.vuejs.org/v2/guide/components-dynamic-async.html](https://cn.vuejs.org/v2/guide/components-dynamic-async.html)

### **keep-alive**

参见：
- [https://cn.vuejs.org/v2/api/#keep-alive](https://cn.vuejs.org/v2/api/#keep-alive)
