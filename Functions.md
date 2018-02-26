# Functions
## What is a Function?

Functions are one of the fundamental building blocks in JavaScript. A function is a JavaScript procedure—a set of statements that performs a task or calculates a value. To use a function, you must define it somewhere in the scope from which you wish to call it.

## Need to Know


A `fuction` is created/called by doing 
```javascript

function doSomething(){ var action= x+1};

```
When you call a function, use camelCase, parentheses and a semicolon: doSomething();

```javascript

var x = function(){}

````



A function can accept things called parameters which are passed in

```javascript

function doSomething(x,y){
}

```

Returning a parameter within a function is done by

```javascript

function doSomething(x,y){
return x*y;
}

```
If the doSomething Function were to be called

```javascript

doSomething(4,6)
24
```


Functions can contain things such as `for` and `if` which are called by
```javascript

function doSomething(x){
for(i=0;i<100;i++){
x+random
  }
}

```

Calling a function is simple. After defining the function, you call it by doing

```javascript

doSomething();

```
# Closures

closures: calling a function with a variable:
 ```javascript
 function myFunc(){
    var c = int(random(0, 255));
    console.log(c); 
    }
    
var colornum = myFunc();
colornum;
```



