# 内置规则

### @import
> 导入css

```css
@import url('./test.css');
@import './test.css';
@import url('http:://test.css');
```

### @charset
> 编码格式

```css
@charset "UTF-8";
```


### @counter-style
> 计数器样式

```css
@counter-style circled-alpha {
  system: fixed;
  symbols: Ⓐ Ⓑ Ⓒ Ⓓ Ⓔ Ⓕ Ⓖ Ⓗ Ⓘ Ⓙ Ⓚ Ⓛ Ⓜ Ⓝ Ⓞ Ⓟ Ⓠ Ⓡ Ⓢ Ⓣ Ⓤ Ⓥ Ⓦ Ⓧ Ⓨ Ⓩ;
  suffix: " ";
}
.items {
   list-style: circled-alpha;
}
```

### @font-face
> 自定义字体;
> format() 这个代表浏览器识别

```css
@font-face {
  font-family: "Open Sans";
  src: url("/fonts/OpenSans-Regular-webfont.woff2") format("woff2"),
       url("/fonts/OpenSans-Regular-webfont.woff") format("woff");
}
```

### @keyframes
> 动画

```css
@keyframes slidein {
  from {
    transform: translateX(0%); 
  }

  to {
    transform: translateX(100%);
  }
}
```

### @support
> 检测

```css
@supports (display: grid) {
  div {
    display: grid;
  }
}
@supports not (display: grid) {
  div {
    display: block;
  }
}
@supports not selector(#id) {
  div {
    display: block;
  }
}
```

### @media
> 响应式网页

```css
@media screen and (min-width: 900px) {
  article {
    padding: 1rem 3rem;
  }
}

/* Nested within another conditional at-rule */
@supports (display: flex) {
  @media screen and (min-width: 900px) {
    article {
      display: flex;
    }
  }
}
```