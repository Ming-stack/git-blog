# 动画

```css
ul{
    /* 保持动画后的样式 */
    /* 3s延迟 */
    animation: opacity ease .2s 3s alternate;

    /* 播放次数 */
    animation: opacity ease 3;

    /* 循环播放 */
    animation: opacity .2s infinite;
}
@keyframes opacity {
    from{
    opacity: 1;
    }
    to{
    opacity: 0;
    }
}
```