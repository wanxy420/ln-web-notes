# ln-web-notes

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

# 链接

|链接|网页名称或类别|
|--|--|
|https://flatuicolors.com/|颜色设计网页|
|https://codepen.io|codepen|
|https://uiverse.io/|组件样式设计|
|https://ask.dcloud.net.cn/article/114|native..js示例|
|https://primevue.org/|vue ui框架|
|https://tinify.cn/|图片压缩|
|https://squoosh.app/|图片压缩|
|https://nuxt.com/|nuxt|
|https://codeantenna.com/a/A5yKoeLhEu|console.log汇总|
|https://zh.geekersoft.com/free-video-converter-online.html|视频转换|
|https://blog.luckly-mjw.cn/tool-show/iconfont-preview/index.html|解析ttf等|
|https://daisyui.com/|daisyUI|
|https://gitee.com/click33/chatgpt---mirror-station-summary|chatgpt汇总|
|https://www.lodashjs.com/|lodashjs|
|https://landing.ant.design/index-cn|官网设计|
|https://auto-animate.formkit.com/|动画|
|https://www.html5plus.org/doc/zh_cn/webview.html|h5+|