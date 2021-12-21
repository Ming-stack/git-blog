# Web Components

### template
> 和vue的很像

```html
<template id="g">
       <div id="nice">
           good
       </div>
</template>
<div id="box">
</div>
<script>
    g.content.querySelector('#nice').textContent = 'Hello'
    const a= document.importNode(g.content,true)
    box.append(a)
</script>
```

### slot
> 和vue很像

```html
<slot name="attributes"><p>None</p></slot>
```