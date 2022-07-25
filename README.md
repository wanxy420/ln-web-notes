# ln-web-notes
## 笔记

#### 对象数据去重

```javascript
let abc = arr1.filter(v=> {
  return arr2.every(val=> {
    return v.id != val.pid
  })
})
console.log(abc)
  
// 方法二
list[index] = list[index].reduce(
	(cur, next) => {
		obj[next.reviewId] ? "" : obj[next.reviewId] = true && cur.push(next);
		return cur;
}, []);
```

#### 数组length报错

> ```javascript
> for (let i = 0; i < (data || []).length ; i++) {
>       // 循环内容
> }
> ```

#### 获取url参数

```javascript
// 获取url参数
function getQueryVariable(variable) {
    var query = window.location.search.substring(1);
    query = decodeURI(query)
    var vars = query.split("&");
    for (var i = 0; i < vars.length; i++) {
        var pair = vars[i].split("=");
        if (pair[0] == variable) {
            return pair[1];
        }
    }
    return (false);
}
```

#### 时间戳转换时间字符串

```javascript
new Date(parseInt(nS) * 1000).
toLocaleString().replace(/:\d{1,2}$/,'')
```
