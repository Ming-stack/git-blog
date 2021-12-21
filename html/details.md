# 细节标签
### blockquote
> 引用...

```html
<blockquote>....</blockquote>
```

### ul & li
> 无序列表

```html
<ul>
    <li></li>
</ul>
```

### ol & li
> 有序列表

```html
<ol>
    <li></li>
</ol>
```

### dl & dt & dd
> 描述列表

```html
<dl>
    <dt></dt>
    <dd></dd>
</dl>
```

### figure & figcaption
> 独立内容：图片，插图，表格，代码段...

```html
<figure>
    <img/>
    <figcaption>说明</figcaption>
</figure>
```


### hr
> 水平线

```html
<hr>
```


### p
> 段落

```html
<!-- 右对齐 -->
<p dir="rtl">test</p>
```

### pre
> 预定义格式文本；
> 可以保留空格和tab格式代码

```html
<pre>
    function a(){

    }
</pre>
```

### a
> 超链接

```html
<a href="http://..." target="_self"></a>
```

### abbr
> 缩写文本

```html
<abbr title="JavaScript">Js</abbr>
```


### b
> 字体加粗

```html
<b>Js</b>
```


### bdi
> 将包含的文本与周围的文本隔离

```html
<bdi>Js</bdi>
```

### bdo
> 改变文字顺序，从右边开始写字

```html
<bdo dir="rtl">Js</bdo>
```

### br
> 强制换行

### wbr
> 屏幕不够时在换行

### cite
> 引用，和那个blockquote的区别在于那个“大”这个“小”

### code
> 程序代码

### data
> 将一个指定内容和机器可读的翻译联系在一起

```html
<ul>
    <li><data value="398">Mini Ketchup</data></li>
    <li><data value="399">Jumbo Ketchup</data></li>
    <li><data value="400">Mega Jumbo Ketchup</data></li>
</ul>
```

### dfn
> 标记了被定义的术语

```html
<dfn><abbr title="JavaScript">js</abbr></dfn>
```

### em
> 重点内容

```html
<em><em>双重点</em></em>
```

### i
> 区分普通文本, 思想活动..

```html
<i>Good<i>
```

### kbd
> 包裹一个键盘符号

```html
<kbd>ctrl</kbd>
```

### mark
> 标记，突出文本

```html
<mark>test</mark>
```

### q
> 引用短文本

```html
<q>small quote</q>
```

### ruby
> 拼音;
> rp包裹括号
> rt包裹字符

```html
<ruby>
    汉<rp>(</rp><rt>han</rt><rp>)</rp>
    子<rp>(</rp><rt>zi</rt><rp>)</rp>
</ruby>
```

### s
> 删除线

### samp
> 计算机程序的输出

### small
> 字体变小

### span
> 和div一个道理，只不过他是行内的

### strong
> 表示文本非常重要

### sub
> 下标

### sup
> 上标

### time
> 时间

```html
<time>20:00</time>
<time pubdate>2019-10-10</time>
<time datetime="2019-10-10 10:00:00">May 5</time>
```

### u
> 下划线

```html
<u>test</u>
```

### var
> 变量的名称