---
title: 兄弟会-第九天--js
published: true　　
---

## js  --定时器

   1 . 一次性定时器　　`setTimeout(tset,2000);`

       ```javascript
function  test(){
    document.body.backgroundcolor="red";
}
setTimeout(test,2000);       
       ```

2 .  周期定时器　　serinterval(test,2000);

3 . 停止定时器　　clearinterval(定时器对象)；

4 . document.getElementByld("id值")　　　通过id值获得唯一对象

5 . document.getElementsByName("name")   通过name对象获得多个对象

6 . document.getElementsByTagName(标签名)   获得多个对象 ,通常用数组接

7 . 三目运算　　`var   x= 3>1?  10:20`

8 . 数组     

```javascript
var   arr=new Array();
arr[0]=10;

```

`var arr =new Array(10,'a',hello);`

`var arr =[1,2,3,4,5];`

9 . 函数

```javascript
function aaa(){
    for  ( var i=0;i<arr.length();i++){
        console.info(i);
    }
}
```

 ```javascript
function   cheng(a,b,c){
    return    a*b*c;
}
var  x=cheng(2,3,4);
alert(x);
 ```

10 . 面向对象

```javascript
var  user   =new  Object();
      user.name="mingren";
      user.age=22;
      user .say=function(){
           alert("我是"+this.name+"你好！");
      }
      user.say();
```

Json对象  ***

```javascript
var  user  ={
  name  :  "mingren",
    age    :21,
    say  : function (){
        alert("你好，我是"+this.name);
    }
}
user.say();   //调用
```

json数组　

```javascript
var  j =[
    { "name":"mingren","age":22},
    {"name":"kakaxi","age":22}
];
alert(j[0].name);
```

json  复杂对象

```javascript
{
    "id":"1111",
        "name":"陈",
            "hobby":["洗脚","洗头发"]
}
```



   



​       











###   





