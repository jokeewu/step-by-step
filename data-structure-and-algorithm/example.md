# 算法实例

### **数字金额正则格式化**

```javascript
'1234567890'.replace(/\d{1,3}(?=(\d{3})+$)/g, ‘$&,’)
"1234567890.11".replace(/\B(?=(\d{3})+(?!\d))/g, ",”)
```

参见：[https://blog.csdn.net/xianzhiding/article/details/86138556](https://blog.csdn.net/xianzhiding/article/details/86138556)