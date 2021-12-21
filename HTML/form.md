# 表单

### button
> 按钮

```html
<button type="button">普通</button>
<button type="reset">重置</button>
<button type="submit">提交</button>
```

### datalist
> 配合input 实现"下拉菜单搜索"功能

```html
<datalist id="data">
    <!-- 可以不用aaa里面的值 -->
    <option value="www">aaa</option>
    <option value="dddd">dddd</option>
</datalist>
<input type="text" list="data">
```

### fieldset & legend
> 可以把一个表单包裹起来，友好显示

```html
<fieldset>
    <legend>登陆</legend>
    <form>...</form>
</fieldset>
```

### form
> 表单元素，自带提交功能

```html
<!-- 
    enctype="application/x-www-form-urlencoded" 默认提交
    enctype="multipart/form-data" 文件上传
    enctype="text/plain"

    novalidate 不要验证表单
    target 和a一样
    autocomplete 记忆功能？
 -->
<form action="提交地址" method="提交方法" enctype="数据格式" novalidate target autocomplete="off/on">
</form>
```

### input
> 各种交互控件

```html
<!-- 
    file,select：
        multiple
    
    type=input:
        pattern="[正则]"
        required
        minlength="4" 
        maxlength="8" 
        size="10"
    
    type: 
        button,checkbox,color,date,datetime-local,
        email,file,hidden,image(带图片的提交),month,
        number, password,radio,range,reset,search,
        submit,tel(移动端友好),text,time,url,week
 -->
```

### label
> 更加友好

```html
<label for="id">点我获取焦点<label>
<input id="id" />
```


### meter
> 复杂版进度条

```html
<!-- 
    
    form="test" test是表单的id 和"那个表单"共同提交 
    optimum="30" 最优值    
-->
<meter
    value="200"
    min="20"
    max="100"
    low="10"
    high="20"
    optimum="30"
    form="test"
>

</meter>
```

### optgroup
> 给option分组

```html
<select id="dino-select">
    <optgroup label="Theropods">
        <option>Tyrannosaurus</option>
        <option>Velociraptor</option>
        <option>Deinonychus</option>
    </optgroup>
</select>
```

### option
> 选项

```html
<option value="test">
<option value="test">1</option>
```

### output
> 计算或者操作的结果

```html
<output name="result"></output>
```

### progress
> 简单进度条

```html
<progress id="file" max="100" value="70"> 70% </progress>
```

### select
> 下拉框

```html
<select multiple>
    <option value="1">name</option>
</select>
```

### textarea
> 文本域

```html
<textarea row="高度" cols="宽度">
</textarea>
```