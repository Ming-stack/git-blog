```js
class Stack{
    list = []
    push(...args){
        this.list.push(...args)
    }
    pop(){
        return this.list.pop();
    }
    peek(){
        return this.list[this.list.length-1]
    }
    isEmpty(){
        return this.list.length === 0
    }
    clear(){
        this.list = []
    }
    size(){
        return this.list.length
    }
}

// 十进制转化二进制
let a = new Stack();
let num = 20;
while(num > 0){
    num % 2 ? a.push(1) : a.push(0);
    num = Math.floor(num / 2);
}
let str = ''
while (!a.isEmpty()) {
    str+=a.pop()
}
```