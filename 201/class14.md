#  Read: 14a - CSS Transforms, Transitions, and Animations

**CSS Transforms**

With CSS3 came new ways to position and alter elements, like transform 
property.


The transform property comes in two different settings, two-dimensional and three-dimensional.

**Transform Syntax**

The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

```html

div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

```

**Dimensional**

Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.Three-dimensional transforms work on both the x and y axes, as well as the z axis.  These three-dimensional transforms help define not only the length and width of an element, but also the depth

The transform property accepts a handful of different values.

**2D Rotate**

The rotate value provides the ability to rotate an element from 0 to 360 degrees
Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise.The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.

```html

<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>



.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}



```

**2D Scale**

Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1.
```html

<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>



.box-1 {
value between .99 and .01 makes an element appear smaller
  transform: scale(.75);
}
value greater than or equal to 1.01 makes an element appear large
.box-2 {
  transform: scale(1.25);
}

```

**2D Translate**

Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.
The distance values used within the translate value may be any general length measurement, most commonly pixels or percentages. 
* Positive values will push an element down and to the right of its default position.

* negative values will pull an element up and to the left of its default position.

for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

![image](https://vuejs.org/images/transition.png)

**Transitional Property**

The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change.

```html
.box {
    background: #2db34a;
    border-radius: 6px
    transition-property: background, border-radius;
    transition-duration: 1s;
    transition-timing-function: linear;
  }

```
**Transition Duration**

The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example

**Transition Timing**

The transition-timing-function property is used to set the speed in which a transition will move. The linear keyword value identifies a transition moving in a constant speed from one state to another. . The ease-in value identifies a transition that starts slowly and speeds up throughout the transition, while the ease-out value identifies a transition that starts quickly and slows down throughout the transition.

**Animations Keyframes**

The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

```html
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}



```

**Animation Name**

the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.

```html
.stage:hover .ball {
  animation-name: slide;
}
```
**Animation Duration,  Timing Function, & Delay**

To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.

```html
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
}
```

A timing function and delay can be declared using the animation-timing-function and animation-delay properties respectively. The values for these properties mimic and behave just as they do with transitions.

![animation](https://media.geeksforgeeks.org/wp-content/uploads/20191115195442/ezgif.com-video-to-gif8.gif)