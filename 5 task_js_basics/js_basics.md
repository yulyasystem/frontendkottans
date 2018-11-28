## JAAAAVAAA SCRIIIPT 
This section can't come soon enough for me and I am here now!
The syntax of JS is similar to other programming languages which I study in my university.

`null` - data type that has no value (value of nothing, totally empty), return null if you purporsely assign value to nothing

`undefined` - absence of value, undefined will be returned if you do not assign value to var

`NaN` returns if you write square root of negative number.

When do such type of convertion `==` or `!=` JS first converts each value to the same type,  better use **strict equality** `====` first compare without type conversion.

The value inside `if` statement is always converted to true or false.

**List of truthy values: **
* false 
* null
* undefined 
* 0
* empty string 
* Nan

Other values are truthy.

*Ternary operator* is shortcut for if statement
```
conditional ? (if condition is true) : (if condition is false)
```
It simplifies the code, but to my mind it is harder to read and understand that code with ternary operator. 
Hoisting in JS hoists function and variable declarations to the top of scope.

When function is stored inside a variable it is called function expression. When function keyword has no name it is called **anonymous**.

A function that is passed into another function is called **callback**. The most common case to pass named function as paramater. Anonymous can be used in event handlers :)

`push` -> add elements to the end of array, returns the length of the array after an element has been added. 

`pop` -> remove elements from the end, returns the element that has been removed

`splice` -> allow to add and remove from anywhere in array 

`forEach` -> manipulate each element of the array

When I was doing exersises on Udacity concerned to array method I tried to use inline function expression with forEach method and that is a little bit tricky. 
`map` -> map returns new array with new values function calculated 

Object in JS is like another data type.

**Naming conventions** for objects. * Do not use numbers as the first charachters in property name, hyphens and spaces* instead use camelCase :)

![image of udacity js](https://github.com/yulyasystem/kottans-frontend/blob/master/5%20task_js_basics\js-basics.png) 

## FreeCodeCamp

**What was new ?**
**Spread syntax** like 3 dots before array, it can be used instead of .apply 
```
Math.max(..arr); 
//instead of
Math.max.apply(null,arr);
```
object `arguments` stores information about parameters

`for ...in` iterates over enumarable properties of object

Ohh, that was not easy, I have been solving tasks for 4 days , but it is great evolution! I learnt a lot of new methods in JS which facilitate a lot. 

![freecodecamp](https://github.com/yulyasystem/kottans-frontend/blob/master/5%20task_js_basics\freecodecamp.png) 










