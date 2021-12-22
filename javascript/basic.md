# JavaScript 语法 

## 数据类型

```js
var test = 'test';
let age = 20;
const SEX = 1;
const obj = {};
const arr = [];
const fn = function(){};
const bool = true;
const n = null;
const u = undefined;
const k = Symbol('');
```

## 语法
```js
// 条件判断
if(true){

} else if(true) {

} else {

}

// 条件判断
let name = 't'
switch(name) {
    case 't': 
        // ....
        break;
    default: 
        // ....
}

// 循环
while(true){}
do{} while(true){}
for(let i=0;i<10;i++){}
for(var i in obj){}
for(var i of [1,2,3]){}

// 类
class Test{
    constructor(){}
}
class Child extends Test{
    constructor(){
        super();
    }
}

// 错误处理
try{
    
}catch(e){

}finally{
    
}
```


