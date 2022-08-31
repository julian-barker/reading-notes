[Home](../README.md)

# Class 14

## CSS Animations

### Transform

- The CSS `transform` property provides a clean way to modify the size and position of elements
- It can be called with various prefixes to maximize browser compatility, with the unprefixed version coming last. These include:
  - `-webkit-`, `-moz`, `-o-`

- `rotate(degrees)` - 2d rotate, taking in degrees as an argument
- `scale(mult)` - scale up/down, taking in a multiplier value as an argument
- `translate(x, y)` - move an element. This could e useful to move elements as you hover them over them, or to create loading animations
  - positive x = right, negative x = left
  - positive y = down, negative y = up

- `skew(x-deg, y-deg)` - distorts elements by a specified number of degrees in the x-axis, y-axis, or both
- multiple types of transforms can be used in a single `transform` property
- `transform-origin` can change the origin point from the dead center of an element to somewhere else. `0 0` signifies the top-left corner
- `perspective` can create depth effects on elements
- `perspective-origin` sets the origin for the perspective property
- `rotateX`, `rotateY`, and `rotateZ` can be used to rotate elements in three dimensions
- `scale` and `tranform` have similar X, Y, and Z variations for 3d versions
- `backface-visibility` sets the visibility of the back of the item, if it is rotated such that the back faces the user. It take take the value `hidden` to make hide an element when facing away.

### Transitions and Animations

#### Transitions

- Transitions allow us to alter the appearance/behavior of an element on state-change, usually via pseudo-selectors such as `:target`, `:hover`, `:active`, `:focus`
- Not all properties can be transitioned, however. Popular transitionable properties are
  - background-color, background-position, border-color, border-width, border-spacing, bottom, clip, color, crop, font-size, font-weight, height, left, letter-spacing, line-height, margin, max-height, max-width, min-height, min-width, opacity, outline-color, outline-offset, outline-width, padding, right, text-indent, text-shadow, top, vertical-align, visibility, widthword-spacing, z-index

- `transition-duration` specifies the amount of time over which a transition should occur
- `transition-timing` sets the speed of a transition
- if tansitioning multiple properties, you can specify multiple timing functions and durations
- `transition-delay` specifies the amount of time before a transition begins

#### Animations

- Animations in CSS3 allow us to specify changes to an element across time using keyframes
- Keyframes specify element state at various points, and the animation propoerty specifies how and when to transition between the keyframes
- We declare keyframes using `@keyframes {}`
  - Each frame is specified with a percentage of the animation, i.e. `0% {background-color: black} 100% {background-color: white}`
- Besides that, animations function largely the same as transitions, accepting duration, timing function, and other values.

### Takeaways

- Transitions and animations are great for making sites feel interactive and engaging, which is a lot of what UI/UX is about
