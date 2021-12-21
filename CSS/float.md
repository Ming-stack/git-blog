# 浮动布局

```css
#div{
    float:left;
}
#div2{
    float:right;
}
#div3{
    float: none;
}

/* 清除浮动bug */
.clear:after{
    content: '';
    clear: both;
    display: block
}
```