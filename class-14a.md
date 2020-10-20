# Class 14b

## Transform

The `transform` property is used to size, position, and change elements in an alternative way. The `transform` property comes in two different settings, `two-dimensional` and `three-dimensional`. Each of these come with their own individual properties and values.

General Syntax:

```css
div {
  -webkit-transform: scale(1.5);
  -moz-transform: scale(1.5);
  -o-transform: scale(1.5);
  transform: scale(1.5);
}
```

### 2D Transform


In 2D Transform , you can rotate, scale, translate items in addition to many other thing.  Using the `scale` value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.
The `rotate` value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.
The `translate` value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.
The `skew` value is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.%p

It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas. Using multiple transform declarations will not work, as each declaration will overwrite the one above it. The behavior in that case would be the same as if you were to set the height of an element numerous times.



Example:

```css
.box-1 {
  transform: scale(.75);
}
.box-2 {
  transform: translateY(25%);
}
.box-3 {
  transform: scale(.5, 1.15);
}
.box-4 {
  transform: skewX(5deg);
}
```

### 3D Transform

As 2D transform, 3D transform has the same values of transform but with a third dimension. For `rotate` we use three new transform values, including rotateX, rotateY, and rotateZ, and by using the scaleZ three-dimensional transform elements may be `scaled` on the z axis. Elements may also be `translated` on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element, while `skew` is the one two-dimensional transform that cannot be transformed on a three-dimensional scale.

## Transition

using `transition` property, you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted. As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover,  `:focus`  , `:active`, and `:target` pseudo-classes.

Some of the transitional Properties

* background-color
* font-size
* opacity
* width
* visibility
* color
* word-spacing

`transition-duration` is The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example. The `transition-timing-function` property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the transition-timing-function property include linear, ease-in, ease-out, and ease-in-out. On top of declaring the transition property, duration, and timing function, you can also set a delay with the `transition-delay` property. The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing

Exampe:

```css

.box {
  background: #2db34a;
  border-radius: 6px
  transition-property: background, border-radius;
  transition-duration: .2s, 1s;
  transition-timing-function: linear, ease-in;
  transition-delay: 0s, 1s;
}
.box:hover {
  background: #ff7b29;
  border-radius: 50%;
}

```

## Animations

To set multiple points at which an element should undergo a transition, use the @keyframes rule. The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated. The `animation-name` property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to. To start, animations need a duration declared using the `animation-duration` property. As with transitions, the duration may be set in seconds or milliseconds. A timing function and delay can be declared using the `animation-timing-function` and animation-delay properties respectively. 

Animations also provide the ability to further customize an element’s behavior, including the ability to declare the number of times an animation runs, as well as the direction in which an animation completes. To have an animation repeat itself numerous times the `animation-iteration-count` property may be used. Values for the animation-iteration-count property include either an integer or the infinite keyword. On top of being able to set the number of times an animation repeats, you may also declare the direction an animation completes using the `animation-direction` property. Values for the `animation-direction` property include normal, reverse, alternate, and alternate-reverse. The `animation-play-state` property allows an animation to be played or paused using the running and paused keyword values respectively. The animation-fill-mode property identifies how an element should be styled either before, after, or before and after an animation is run. The animation-fill-mode property accepts four keyword values, including none, forwards, backwards, and both.

Example:

```css
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
  animation-fill-mode: forwards;
}
.stage:active .ball {
  animation-play-state: paused;
}

```

[Back to Home](README.md)
