#### 一、变量

1. ##### 声明变量	 

​		在JavaScript中，使用变量之前必须要提前**声明**（使用 let 或 var），可以不用声明**变量类型**（动态类型）。

```javascript
let name = 'Oliver';
let age = 12;
var high = "168cm";
```

​	注：关于 let 和 var 区别，看[MDN](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/First_steps/Variables)。

##### 		2 .变量类型

​		变量包含：数字（Number），字符串（String），布尔（Boolean），数组（Array），对象（Object）

```javascript
let Myage = 12;

let name = "Oliver";

let iAmAlive = true;
let test = 6 < 3;

let myNameArray = ['Chris', 'Bob', 'Jim'];
myNameArray[2]  // return "jim"

let dog = { name : 'Spot', breed : 'Dalmatian' };
dog.name  // return "Spot"
```

- ##### 数组使用

```javascript
# 创建数组，数组值的类型可以包含任意变量类型
let sequence = [1, 1, 2, 3, 5, 8, 13];
let random = ['tree', 795, [0, 1, 2]];

# 获取数组长度,通过数组的 .length属性
sequence.length;

# 遍历数组
for (let i = 0; i < sequence.length; i++)
{
    console.log(sequence[i]);
}
```

​	字符串与数组之间的转换  **split() 和 join()**

```javascript
# 字符串转换为数组
let myData = "Manchester,London,Liverpool,Birmingham,Leeds,Carlisle";
let myArray = myData.split(','); # 用 "," 来分割字符串成为数组
myArray

# 数组转换为字符串
let myNewString = myArray.join(','); # 用 "," 分隔符来拼接数组成为字符串

let dogNames = ["Rocket","Flash","Bella","Slugger"];
dogNames.toString(); //return : "Rocket,Flash,Bella,Slugger"

```

​	添加和删除数组 **push()** 和 **pop()** 、**unshift()** 和 **shift()** 

```javascript
# push() 在数组尾端添加元素
let nums = [1, 2, 34, 41, 21]
nums.push(98)
nums;	# return : (6) [1, 2, 34, 41, 21, 98]

# pop() 删除数组尾端元素
nums.pop();
nums;

# unshift() 和 shift() 作用于数组开始
let words = ['good', 'bad', 'well'];
words.unshift("Just so so"); # return : (4) ["Just so so", "good", "bad", "well"]

words.shift();
words;
```

#### 二、注释

- 单行注释，使用双斜杠 **//**

```javascript
// 我是一条注释
```

- 多行注释，使用 **/* 和 */**

```javascript
/*
  我也是
  一条注释
*/
```

#### 三、使用Python来执行Js代码

使用**js2py**模块，官方github文档：[js2py](https://github.com/PiotrDabkowski/Js2Py)

```python
# 简单使用说明
import js2py

In [66]: js2py.eval_js("console.log('Hello World')")
'Hello World'

In [67]: js2py.eval_js("let name ='Oliver'")
Out[67]: 'Oliver'

# 多行代码使用
>>> js = js2py.EvalJs()
>>> js.execute('var a = 10; function f(x) {return x*x};')
>>> js.f(9)
81
>>> js.a
10
```

