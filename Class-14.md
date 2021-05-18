## Transforms
### With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

### The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

### Within this lesson we’ll take a look at both two-dimensional and three-dimensional transforms. Generally speaking, browser support for the transform property isn’t great, but it is getting better every day. For the best support vendor prefixes are encouraged, however you may need to download the nightly version of Chrome to see all of these transforms in action.

## Transform Syntax
### The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

```
CSS

div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```

## 2D Transforms
### Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.

## 2D Rotate
### The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.


```
HTML

<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>

```

```
CSS

.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}

```

## References : in the previous info about transforms I relied on [advanced-html-css-transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

--------------------------------------------------------------------------

## Transitions & Animations

### One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

### With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

### Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

### Transitions
### As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

### There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

### In the example below the box will change its background color over the course of 1 second in a linear fashion.

```
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```

### Vendor Prefixes
### he code above, as with the rest of the code samples in this lesson, are not vendor prefixed. This is intentionally un-prefixed in the interest of keeping the code snippet small and comprehensible. For the best support across all browsers, use vendor prefixes.

### For reference, the prefixed version of the code above would look like the following.

```
.box {
    background: #2db34a;
    -webkit-transition-property: background;
       -moz-transition-property: background;
         -o-transition-property: background;
            transition-property: background;
    -webkit-transition-duration: 1s;
       -moz-transition-duration: 1s;
         -o-transition-duration: 1s;
            transition-duration: 1s;
    -webkit-transition-timing-function: linear;
       -moz-transition-timing-function: linear;
         -o-transition-timing-function: linear;
            transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```

### Transitional Property
### The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

### In the example above, the background property is identified in the transition-property value. Here the background property is the only property that will change over the duration of 1 second in a linear fashion. Any other properties included when changing an element’s state, but not included within the transition-property value, will not receive the transition behaviors as set by the transition-duration or transition-timing-function properties.

### If multiple properties need to be transitioned they may be comma separated within the transition-property value. Additionally, the keyword value all may be used to transition all properties of an element.

```
.box {
    background: #2db34a;
    border-radius: 6px
    transition-property: background, border-radius;
    transition-duration: 1s;
    transition-timing-function: linear;
  }
  .box:hover {
    background: #ff7b29;
    border-radius: 50%;
  }
```


## Animations
### Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

### Animations Keyframes
### To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

``` 
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


### The animation above is named slide, stated directly after the opening @keyframes rule. The different keyframe breakpoints are set using percentages, starting at 0% and working to 100% with an intermediate breakpoint at 50%. The keywords from and to could be used in place of 0% and 100% if wished. Additional breakpoints, besides 50%, may also be stated. The element properties to be animated are listed inside each of the breakpoints, left and top in the example above.

### It is important to note, as with transitions only individual properties may be animated. Consider how you might move an element from top to bottom for example. Trying to animate from top: 0; to bottom: 0; will not work, because animations can only apply a transition within a single property, not from one property to another. In this case, the element will need to be animated from top: 0; to top: 100%;.

```
.stage:hover .ball {
  animation-name: slide;
}
```

### Animation Duration, Timing Function, & Delay
### Once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.

```
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
}
```
### A timing function and delay can be declared using the animation-timing-function and animation-delay properties respectively. The values for these properties mimic and behave just as they do with transitions.

```
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
}
```


## References: In Transitions & Animations Section I relied on [advanced-html-css/transitions-animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)