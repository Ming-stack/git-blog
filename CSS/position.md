# 定位布局

> 子绝对父(相对,固定,绝对)
```css
#div{
    /* 要有参照物 */
    position: absolute;

    /* 默认整个页面 */
    position: fixed;

    /* 相对定位 */
    position:relative;

    /* 粘性定位: 比如一个元素设置了这个属性, 滚动条超过最高元素 就被固定 */
    position: sticky;

    /* 默认 */
    position: static;

    /* 层级 */
    z-index: 10;
}
```