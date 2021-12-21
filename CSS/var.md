# CSS变量

```css
:root{
    /* 全局变量 */
    --main: red;
}
div{
    /* 使用 */
    color: var(--main);
}
```

### 计数器

```css
body {
  counter-reset: section;
}
 
h2::before {
  counter-increment: section;
  content: "Section " counter(section) ": ";
}
```