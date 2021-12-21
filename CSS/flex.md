# Flex布局

```css
div{
    /* 块级 */
    display: flex;

    /* 内联 */
    display: inline-flex;

    /* 排列方式 默认 横轴 */
    flex-direction: row;

    /* 横轴逆序 */
    flex-direction: row-reverse;

    /* 纵轴 */
    flex-direction: column;

    /* 纵轴逆序 */
    flex-direction: column-reverse;

    /* 需要换行 */
    flex-wrap: wrap;

    /* 简写 */
    flex-flow: row wrap;

    /* 设置垂直对齐方式 */
    align-items: center;
    align-items: flex-end;
    align-items: flex-start;

    /* 设置水平对齐方式 */
    justify-content: center;
    justify-content: flex-end;
    justify-content: flex-start;
}

/* 子元素 */
.child{
    /* 设置宽度 */
    flex-basis: 100px;

    /* 设置宽度 */
    flex-grow: 2;

    /* 设置宽度 */
    flex-shrink: 1;

    /* 缩写 */
    flex: 1;
}
```