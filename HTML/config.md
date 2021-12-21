# 控制全局标签
### html
> 网页根元素，所有的内容在这里面输出

```html
<html></html>
```

### head
> 配置浏览器的一些信息

```html
<head></head>
```

### body
> 网页的主要内容

```html
<body></body>
```

### base
> 指定页面上所有的a标签的属性, 必须要加http;
> a标签的href属性是相对href就能生效，否则覆盖默认;
> 如果页面上有多个只会使用第一个的;

```html
<base href="http:/api/v1" target="_self">
```

### link
> 链接外部css

```html
<link rel="stylesheet" href="/">
```

### meta
> 可以设置浏览器的功能

```html
<!-- 浏览器字符编码 -->
<meta charset="utf-8">
<!-- 3秒之后重定向 -->
<meta http-equiv="refresh" content="3;url=https://www.mozilla.org">
```

### style
> 內联css

```html
<style>
    html{
        font-size: 20px;
    }
</style>

```

### title
> 设置浏览器标题

```html
<title>标题</title>
```
