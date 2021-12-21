# 背景

```css
.one{
   /* 背景颜色 */
   background-color: red;

   /* 背景图片 */
   background-image: url(/test.jpg), url(/test.jpg);

   /* 背景图片定位 */
   background-position: 20px 20px, 30px 30px;

   /* 背景图片大小 */
   background-size: 20px 20px, 30px 30px, cover, contain;

   /* 背景平铺 */
   background-repeat: repeat-x, repeat-y, no-repeat;

   /* 线性渐变 */
   background-image: 
    linear-gradient(45deg, blue, red),
    linear-gradient(to right, blue, red),
    linear-gradient(to left top, blue, red);

    /* 迳向渐变 */
    background-image:  radial-gradient(blue, red);

    /* 背景裁减 */
    background-clip: border-box,padding-box,content-box;

    /* 显示的位置 */
    background-orgin: border-box,padding-box,content-box;

    /* 背景图片固定不动 */
    background-attachment: fixed;

    /* 背面不可见 */
    backface-visibility: hidden;
}
```