# 优化

代码、架构、流程

### **性能优化**

#### 代码层面

* 代码（组件）复用
* 代码（代码片段、组件）性能优化，`参考具体框架优化方案`
* 去掉无用代码，如：Tree shaking，`参考Webpack`
* DNS prefetch（DNS预解析）

#### 浏览器端

* 缓存，如：数据缓存xxxStorage、304
* 减少请求头，如：Cookies

#### 服务器端

* [CDN](https://baike.baidu.com/item/CDN/420951?fr=aladdin)
* GZip
* 缓存，如：业务数据、模版等
* 首屏渲染
* BFF（Backend For Frontend）

#### 资源文件

* 图片压缩（图片格式，压缩方案？）
* JS/CSS等压缩
* 文件名hash

F5/Command+Shift+R区别/强制刷新区别

参考资料：

* https://www.cnblogs.com/slly/p/6732749.html
* https://www.cnblogs.com/etoah/p/5579622.html
* https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Caching_FAQ

---

### **如何重构**
