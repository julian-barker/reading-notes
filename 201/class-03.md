[Home](../README.md)

# Class 03

## HTML

- HTML uses what's called "markup" to annotate content for display
- To do this, it uses elements to contain contain.
- Elements can be semantic, in that they convey some meaning about the content enclosed, or they can be generic

### Ordered Lists

- Ordered lists display contained list items in a list format, typically with a preceding marker. They differ from unordered lists in that the order or sequence of items is meaningful
- Permitted content: `<li>`, `<script>`, `<template>`
- Attributes:
    - `reversed` - displays the items in reverse order (high->low)
    - `start` -  specify the starting point to count from (always a number, regardless of the numeral type)
    - `type` - sets the numeral type:
        - `a` - lowercase letters
        - `A` - UPPERCASE letters
        - `i` - lowercase roman numerals
        - `I` - UPPERCASE roman numerals
        - `1` - numbers (default)

### Unordered Lists

- similar to ordered lists, but without meaning to the order of elements
- `type` - sets the symbol type: `circle`, `disc`, `square`

## CSS

- Everything in CSS has a box around it
- Two types of boxes - inline boxes and block boxes (set with the `display` property)
- `block` boxes break onto a new line and respect width/height properties
    - padding, margin, border will push outwards
- `inline` boxes do not break onto a new line and width/height propoerties do not apply
    - horizontal padding, margin, border will push other inline boxes away
- `<a>`, `<span>`, `<em>`, `<strong>` all use `inline` as the default `display` property
- `flex` is an inner display type that effects items within the box. The outer display type remains `block`
- `grid` is another inner display type
- The content box contains the content and can be sized with the `height` and `width` properties
- `border` creates a border around the content
- `margin` determines how far away from other elements a given element sits (space around the `border`)
- `padding` determines how far away from the content that element's `border` is (space within the `border`)

## Learn JS

- Arrays can store basically any data type, such as numbers, strings, other arrays, and objects

 > const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

- The above array `people` is a valid array, and you can access its elements using bracket notation. Access elements in nested arrays using an additional set of brackets. (i.e. `people[0][2]` would return `'librarian'`)
- Shorthand assignment operators make for cleaner and quicker code
    - `+=` is the same as `x = x + y`
    - `-=`, `*=`, `/=`, `**=`, and `%=` thus all function in the same pattern as `+=`
- The expression `(10 + false) + 'dog'` evaluates to '10dog' because the false is falsy, which can be evaluated to zero for mathematical purposes, resulting in 10. 10 then gets converted to a string ('10') to concatenate with 'dog', resulting in '10dog'
- A conditional can be used inside a javascript program to validate input from a user. For example, if an input field asks for a number input, we can use conditionals and the isNaN function to prevent any inputs that are not numbers
- Loops are useful in Javascript when we need to perform repetetive actions, either for a predetermined time, for all values in an array, for an undetermined amount of time until a condition is met, etc.
    - An example would be accessing a stored array of test scores for a class to add them all together and take the average (Note: this specific example can be done more easily with the .reduce method)
