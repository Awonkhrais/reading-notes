# **Transforms**

The `transform` property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

The `transform` property applies a 2D or 3D transformation to an element. This property allows you to rotate, scale, move, skew, etc., elements.

![transform](https://cdn.codecoda.com/images/made/images/breadcrumb/css-transform-banner_1543_592_40.jpg)


## 2D Transforms 

* **Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.**

### 1. 2D Rotate : 

* The `rotate` value provides the ability to rotate an element from 0 to 360 degrees.

* Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise.

* The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.


### 2. 2D Scale :

* Using the `scale` value within the transform property allows you to change the appeared size of an element. 

* The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

* It is possible to scale only the height or width of an element using the scaleX and scaleY values.

HTML
``` html
<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>
<figure class="box-3">Box 3</figure>
```

CSS
```CSS
.box-1 {
  transform: scaleX(.5);
}
.box-2 {
  transform: scaleY(1.15);
}
.box-3 {
  transform: scale(.5, 1.15);
}
```

### 3. 2D Translate :

* The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.

* Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

* Positive values will push an element down and to the right of its default position while negative values will pull an element up and to the left of its default position.

### 4. 2D Skew :

*  `skew`, is used to distort elements on the horizontal axis, vertical axis, or both.

## 3D Transforms 

* **Using three-dimensional transforms we can change elements on the z axis, giving us control of depth as well as length and width.**

----------------------

# Transitions & Animations.

## Transitions

With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

The easiest way for determining styles for different states is by using the `:hover`, `:focus`, `:active`, and `:target` pseudo-classes.

There are four transition related properties in total, including transition-property,transition-duration,transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.


## Animation Direction: 
 By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the `animation-iteration-count : infinite` property may be used.

 ![animation](https://hackernoon.com/drafts/x84g2geg.png)


* Animation Keyframes : To set multiple points at which an element should undergo a transition, use the `@keyframes` rule. The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

* Animation Iteration : By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the `animation-iteration-count : infinite` property may be used.


* Animation Direction : On top of being able to set the number of times an animation repeats, you may also declare the direction an animation completes using the `animation-direction` property. Values for the `animation-direction` property include `normal`, `reverse`, `alternate`, and `alternate-reverse`.