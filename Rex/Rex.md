### 每隔四位数字中间用空格
```javascript
let str = "128931723487427873842734823";
let rex = str.replace(/\s/g, '').replace(/(.{4})/g, "$1 ");
alert(rex);
```