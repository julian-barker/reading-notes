[Home](../README.md)

# Class 04

## Creating hyperlinks

1. To create a link, we wrap content inside the `<a>` element.
2. The `href` contains the URL for the link, while the content of the tag is the text displayed
    - ex. `<a href="https://www.facebook.com/">hamsters</a>` would display as [hamsters](https://www.facebook.com/) but take you to facebook.com
3. We can ensure our links are accessible by clearly stating where the link leads in the content, and also putting a `title` attribute in the `<a>` tag

## CSS Normal Flow and Positioning

1. Normal flow describes the way an HTML documents contents are laid out without any external styling.
2. Inline vs block-level elements:
    - A block level element fills the inline space of its parent element. By default, block-level elements appear in the block flow direction, which by default places each block on a new line under the previous block, separated by margins.
    - An inline element is the size of its content. Unlike block level elements, you cannot set their width and height. By default, inline elements sit next to each other
3. Positioning allows us to override the default flow of a document. It's changed with the `position` property. Static positioning is the default for every HTML element. Relative positioning allows an element to be placed somewhere relative to where it would sit by default, by adding space to one or more sides.
4. Absolute positioning is uesful to create elements that do not interfere existing elements. Examples could be popup windows, UI features, some menus, etc.
5. Absolute positioning causes an element to sit outside of the normal flow of the rest of the elements. Instead, it is positioned relative to it's container element on a separate layer from everything else.

## Javascript Functions

- Functions allow us to execute complex code and gives us the ability to reuse that code multiple times!

1. A function declaration creates the function, so that it can be invoked. It identifies the code to run, and the input parameters required. A function invocation calls and executes the function with supplied arguments.
2. A parameter is defined for a function at declaration, while an argument is supplied to a function at invocation. Both refer to user-supplied inputs

## Pair Programming

1. Pair programming provides 6 key advantages
    - Greater efficiency: it is much easier to catch mistakes and produce high-quality code
    - Both programmers are more focused
    - Both programmers can learn from each other
    - Pair programming improves social skills important to working on teams
    - Pair programming helps prepare for potential job interviews
    - Pair programming is frequently used for new hires, so being accustomed to it can prepare you to be off to a good start in a new job
