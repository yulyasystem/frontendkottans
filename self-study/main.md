## JS Modules
> Good authors divide their books into chapters and sections; good programmers divide their programs into modules.

I want to explore this part of JS, because I've realized its benefits. Code can be split into smaller logical functionality files, the same modules can be shared and reused. While many scripts tags in html affects performance, because each script initiaties HTTP request, and it is hard to maintain. The solution is concantenation. Bundlers introduce compiler step, the build procsess has benefits. We can have proccess  to be automated, it also can minimify files. I tnink that is great to oprimize development procces, to make automative routines and enjoy solving problems (or not:) 

### ES6 Modules 
Everything inside modules are private and runs in strict mode. Public vars and funcs are shared by `export` :

```js
export function kottans(){
  console.log("You are awesome!");  
}

export const KOTANS = "Knowledge must be shared!";
```
also we can use single export like 
```js
export  {KOTANS, kottans}
```
import is used to pull items into another modules like:
```js
import {kottans} from './kottans.js';
```
  all public items can be imported by providing namespace:
  ```js
import * as kotik from './kottans.js';
console.log(kotik.meow());
```
As I properly understand due to poor browser support better to use module bundlers. The most popular is webpack.    

Such strange feelings when using webpack. I use `--mode development` optimizes for build speed, and `--mode production` optimizes for execution speed, also minimify files :) Imports without relative path like `es-lodash` are modules from npm, my own modules need to be like `./module`



