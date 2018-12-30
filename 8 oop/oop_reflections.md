Course on Udacity was too hard to percieve information, so I try reading learn.javascript.ru 
![image of udacity js](https://github.com/yulyasystem/kottans-frontend/blob/master/8%20oop/udacity_oop.png) 

In order to avoid repetable code when create objects we can use constructors : 

```
function Book(title,author){
    this.title = title;
    this.author = author;
}
```
It is like blueprint. We can place spesific methods of object in the prototype rather than in object itself.

```javascript
Book.prototype.getSummary = function(){
    return `${this.title} was written by ${this.author}`;
```
Inheritance is realized as 
```js
 function.call(thisArg, arg1, arg2, ...)
  ```
*ES6 classes* support prototype inheritance, constructors, calls. 

```js
class Book{
    constructor(title,year,author){
        this.title = title;
        this.year = year;
        this.author = author;
    }
    getSummary(){
        return `${this.title} was written by ${this.author}`
    }
}
```
I think  it is easier to use. 

7kyu is achieved :) 

![codewars](https://github.com/yulyasystem/kottans-frontend/blob/master/8%20oop/7kyu.png) 

