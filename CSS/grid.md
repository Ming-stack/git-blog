# 网格布局


```css
.parent{
    display: grid;

    /* 第一种设置宽高 */
    /* 3列的宽度 */
    grid-template-columns: 100px 100px 100px;
    grid-template-columns: 1fr 1fr 1fr; 
    grid-template-columns: repeat(3,1fr);

    /* 3行高度 */
    grid-template-rows: 100px 100px 100px;
    grid-template-rows: 1fr 1fr 1fr; 
    grid-template-rows: repeat(3,1fr);

    /* 第二种设置宽高 */
    grid-auto-columns: minmax(auto, 1200px);
    grid-auto-rows: minmax(auto, 1200px);

    /* 设置间距 */
    grid-column-gap: 10px;
    grid-row-gap: 1em;

}
.child{
    /* 跨列,跨行 */
    grid-column-start: 1;
    grid-column-end: 4;
    grid-row-start: 1;
    grid-row-end: 3;
}
```