# Responsive Web Design
Make content work across any device.

 Device Independent Pixels (relates pixels to real distance), dpi will take up the same amount of space on display regardless of the pixel density of the display. With one dip for every two hardware pixels, the device pixel ratio is 2.
To calculate CSS pixels= hardware pixels / device pixel ratio. 

**What was new for me?**

That is ability to debug on my smartphone, switching on developer mode, also I found out new features on my phone in developer options, thanks udacity :smirk:

`max-width` if the content is larger than max width it will change the height of element. it overrides width property

`min-width` if the content is smaller than min widht, it will be applied, never become smaller than min
 
 **Media-queries** apply style depending on device chars like its widht, height.

 ```
 @media screen and (min-width:500px) and(){
     body{
         background-color: green;
     }
 }
 ```
 I have already had experience with Flexbox. And it is awesome! I love it. And I`m surely will intend it in my projects.

![image of udacity responsive](https://github.com/yulyasystem/kottans-frontend/blob/master/4%20task_responsive_web_design/web-responsive-udacity.png)

 I found out Udacity course too easy and want to read more about Flexboxes, Grids. I read [nice article](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) on css-tricks with cool pictures which clearly describe flexbox principles. 
## Flexbox

```
.container{
    display:flex;
}
```
defines flext container and enables flex to all direct children. `flex-wrap` defines will items be in one line or wrapped

One thing that tangle me up a little is axes in rows and columns with `justify-content` and `align-items`. 

`justify-content` - alignment alon main axes, `align-tems` - alons cross 

```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
}
```
`align-self` overrides align-items, define alignment alon cross axes for individual item

`flex-flow` applies to parent container, combine `flex-direction` and `flex-wrap`.

Align-* is for cross axis and justify for main axis. If you set your direction row, so it is your main axis, if you set direction column it is your main axis. Easy! 

Frogs game is interesting and funny! I wanna more :) Froges brought home:

![image of udacity responsive](https://github.com/yulyasystem/kottans-frontend/blob/master/4%20task_responsive_web_design/froggy.png) 

I have tried to practice with responsive and it is only seems easy, until you write your own media querie and get confused with min and max-width :smile: 






