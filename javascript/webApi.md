# 浏览器提供的API

## 基础dom操作

```js
// 基础dom操作
const body = document.querySelector('body');
body.parentNode;
body.children;
body.childNodes;
body.getAttribute('id');
body.classList.contain('test')

window.innerWidth;
window.innerHeight;

document.body;
document.documentElement;

document.body.appendChild(newNode);
document.body.append(newNode, newNode2);

document.querySelector('div').remove();
document.querySelector('div').removeChild(childNode);
body.removeAttribute('id');
body.classList.remove('')

const body = document.querySelector('body');
body.innerHTML = '<div>test</div>';
body.innerText = 'text';

body.id = 'mybody';
body.className = 'test';

body.setAttribute('data', 'test');
body.classList.toggle('test')

const p  = document.createElement('p');
const text = document.createTextNode('test');
body.classList.add('test', 'test');

document.body.onclick = function(e){
    e.stopPropagation();
    e.target;
}
document.body.addEventListener('click', fn);
document.body.removeEventListener('click', fn);
window.onscroll = function(){
    window.scrollX;
    window.scrollY;
}
```

## 通用API

### Date
> 时间日期操作
> UTC: 世界标准时间

| Date.parse()              | 传入一个字符串,返回一个时间戳       |
| ------------------------- | ----------------------------------- |
| Date.UTC()                | 传入一个指定参数,返回一个本地时间戳 |
| Date.now()                | 返回当下的时间戳                    |
| date.getTime()            | 返回当下的时间戳                    |
| date.setTime()            | 设置当下的时间戳                    |
| date.getFullYear()        | 返回当下的年                        |
| date.setFullYear()        | 设置当下的年                        |
| date.getMonth()           | 返回当下的月                        |
| date.setMonth()           | 设置当下的月                        |
| date.getDate()            | 返回当下的日                        |
| date.setDate()            | 设置当下的日                        |
| date.getDay()             | 设置当下的星期                      |
| date.setDay()             | 设置当下的星期                      |
| date.getHours()           | 设置当下的小时                      |
| date.setHours()           | 设置当下的小时                      |
| date.getMinutes()         | 设置当下的分钟                      |
| date.setMinutes()         | 设置当下的分钟                      |
| date.getSeconds()         | 设置当下的秒钟                      |
| date.setSeconds()         | 设置当下的秒钟                      |
| date.getMilliseconds()    | 设置当下的毫秒                      |
| date.setMilliseconds()    | 设置当下的毫秒                      |
| date.toLocaleDateString() | 返回本地年月日格式字符串            |
| date.toLocaleTimeString() | 返回本地时分秒格式字符串            |
| date.toDateString()       | 返回本地年月日格式字符串            |
| date.toTimeString()       | 返回本地时分秒格式字符串            |
| date.toUTCString()        | 返回本地时年月日分秒格式字符串      |
| date.toString()           | 返回本地&当下年月日分秒格式字符串   |


### RegExp
> 正则匹配

#### flag

|  /\.test/ig   | 简洁语法  |
|  i  | 不区分大小写  |
| g  | 全局匹配 |
| m  | 多行模式 |
| y  | 粘附模式 |
| u | Unicode模式 |
| s | dotAll模式 |

#### Symbol

|  ()   | 分组  |
|  .  | 任意  |
| *  | 0或多 |
| +  | 1或多 |
| ^  | 开头 |
| $ | 结尾 |
| ? | 0或1 |
| [a-z] | a-z任意一个 |
| [0-9] | 0-9任意一个 |
| [0-9]{2,} | 0-9 2个+ |

#### API

|  new RegExp("[a-z]", "i")   | 构造函数创建  |
|  reg.gloabl  | 是否设置g  |
|  reg.ignoreCase  | 是否设置i |
|  reg.unicode | u |
|  reg.sticky | y |
|  reg.lastIndex | 下一次开始搜索的位置 |
|  reg.multiline | m |
|  reg.dotAll | s |
|  reg.source | "[a-z]" |
|  reg.flags | "i" |
|  reg.exec(text) | 如果正则有括号,返回的数组可以[0]直接访问 |
|  reg.matches(text) | 匹配到[0]访问, 否则null |
|  reg.test("1,2,3") | 返回true,false |
|  RegExp.$1 | 需要配合reg.test(), $1代表第一个括号分组匹配 |

### String
> 字符串

### Number
> 数字

### Object
> 对象

### Array
> 数组

### Set
> 集合

### Proxy
> 代理

### Map
> 映射


## Web API

### MutataionObserver

> 监听dom改变

```js
var observer = new MutationObserver((a) => {
})
// 观察多个
observer.observe(box, { attributes: true, childList: true })
observer.observe(txt, {
    attributes: true, 
    childList: true, 
    subtree: true, 
    attributeFilter: ['id'],
    attributeOldValue: true,
    characterData: true,
    characterDataOldValue: true,
})
// 取消观察
observer.disconnect();
```

### 自定义事件

```js
 var custom = document.createEvent('MouseEvents');
 var custom = document.createEvent('KeyboartEvent');
custom.initMouseEvent('click', true, true, document.defaultView, 0, 0, 0, 0, 0, false, false, false, false, 0, null);
document.body.dispatchEvent(custom)

 var custom = document.createEvent('KeyboardEvent');
custom.initKeyboardEvent('keydown', true, true, document.defaultView, 0, 0, 0, 0, 0, false, false, false, false, 0, null);
document.body.dispatchEvent(custom)

var custom = document.createEvent('HTMLEvents');
custom.initEvent('focus', true, true,false);
document.body.dispatchEvent(custom)

var custom = document.createEvent('CustomEvent');
custom.initCustomEvent('focus', true, true,false);
document.body.dispatchEvent(custom)
```