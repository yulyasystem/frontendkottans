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

### Sizing in CSS Layout

Font relative unit `rem` is always relative to the `root element`. For example, html is root element, it has font-size 20px, therefore 1rem == 20 pixels, when give an element width of 10rem it will become 200px wide. Other unit like `em` is relative to thee font size that is applied to an element  like font-size of element is 40px and the width is 10em, so the width is 400px. 

`Viewport` is part of webpage that the user can currently see.  Varies on the devices.

`Viewport relative units` are calculated in relation to initial containing block, on the screen it is viewport. The `vw` is 1/100 of width of viewport, `vh` the same with height. 

`vmin` and `vmax` is usufel when configure landscape and portrait modes. If the device is held in the portrait mode then 20vmax would be the same as 20vh, same for lanscape.

Div  is block level element, if you dont give the size to this element , it will be as wide as it can in inline dimension. `width:min-content` on the div, it becomes as large as it needs to be with content becoming as small as inline direction as possible. Does not caause overflow. But opposite  `max-content` cause overflow. `fit-content` works like max-content but here we can set the wrap point like `fit-content(100px)`

### Grid
Grid elements can be placed on page using:
 * numbered lines. `grid-column:7/13` is set to be placed from 7 to 13 line, the same with rows. 

 * names lines. name lines like 
 ```css
  grid-template-columns:[full-start] 1fr [content-start] 30em [content-end]1fr [full-end];   
 ```  
  ` grid-columns:content-start/content-end`
  * grid-template-areas
```css
    grid-template-areas: 
            "aside header ."
            "aside text ."
            ". text text";
  ```
  points are like gaps. I think it makes code much more simple

We can span 2 rows together like :
 ```css
 .class{
     grid-row:span 2;
 }
```

*Grid works on direct children*. There can be an issue with lists, `<li>` is not direct child of grid container and it cant play grid game :(  The rescue is `display:content`. Every element in the documnet tree is rectangulat box consist of 2 sections. Actual box - border,padding,margin, and content of the box like text inside. We can control about how box and its children will be drawn on the page. CSS rule only affects the box being visually drawn on the page, it does not affect the markup. I understand it like we ommited closing tag, it is cool to save semantic rules. But there are issues with accesibility, in some browsers it can not render properly.





