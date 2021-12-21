# 选择器

## 一般选择器

```css
/* id */
#one{}
/* class */
.one{}
/* attribute */
[name="age"]={}
/* tagname */
input{}
```


## 伪类选择器

```css
/* a标签4中状态 */
a:link{}
a:visited{}
a:hover{}
a:active{}

a:first-of-type{}
a:last-of-type{}
/* 单数 */
a:nth-of-type(odd){}
/* 双数 */
a:nth-of-type(even){}
a:focus{}

/* "之前"的一个元素 */
div::before{
    content: ''
}
div::after{
    content: ''
}
/* 选区 */
body::selection{

}

/* html */
:root{}
input:placeholder{}

/* 排除 */
div:not(.name){}

/* 字幕 */
video::cue{}

/* 选择影子节点树下的 */
::slotted(*) {
  font-weight: bold;
}
```

## 组合选择器

```css
/* 兄弟选择器 */
img + p {}
/* 并集选择器 */
img, p {}
/* 后代选择器 */
div p {}
```