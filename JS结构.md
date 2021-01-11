### 一、条件语句结构

####  1.if...else 语句

- ##### 在 **if** 条件语句中，else语句可以忽略。

```javascript
if (condition) {
  code to run if condition is true
} else {
  run some other code instead
}
```

```javascript
if (condition) {
  code to run if condition is true
}

run some other code
```

```javascript
if (condition) code to run if condition is true
else run some other code instead
```

- ##### **else if**

```javascript
if (A) {
    code to run if A condition is true;
}else if (B) {
    code to run if B condition is true;
}else if (C) {
    code to run if C condition is true;
}else{
    code to run if A、B、C condition is false;
}
```

- ##### 嵌套if...else

```javascript
if (A){
    if (B){
        code to run if A、B condition is true
    }else{
        code to run if A condition is true, B condition is false
    }
}else{
    code to run if A、B condition is false
}
```

- ##### 逻辑运算符

```javascript
/#
1. && ---逻辑与
2. || ---逻辑或
3. !  ---逻辑非
#/
```

####  2. switch语句

```jade
switch (expression) {
  case choice1:
    run this code
    break;

  case choice2:
    run this code instead
    break;

  // include as many cases as you like

  default:
    actually, just run this code
}
```

####  3. 三元运算符

```javascript
( condition ) ? run this code : run this code instead
```

### 二、循环语句结构

####  1. for

```javascript
for (initializer; exit-condition; final-expression) {
  // code to run
}
```

####  2. while

```javascript
initializer
while (exit-condition) {
  // code to run

  final-expression
}
```

####  3. do...while

```javascript
initializer
do {
  // code to run

  final-expression
} while (exit-condition)
```





