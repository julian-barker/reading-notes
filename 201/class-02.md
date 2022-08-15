[Home](../README.md)

# Class 02

## HTML Text Fundamentals

- All text is wrapped in elements (`<p></p>`, `<h1></h1>`, etc.)
- There are six heading types: `h1` - `h7`
- You can assign each level of heading to whatever you want, but the hierarchy should make sense
    - ex. `h1` for the main site title, `h2` for section titles, `h3` for subsection titles
- Structure allows for easy navigation of our sites and allows visually impaired site visitors to obtain structural information that would normally be conveyed visually with the help of a screen reader
- Structure allows for effective, targeted styling and function in CSS and Javascript
- Semantic elements provide us with some default styling and the ability to be screen-reader compatible
    - We can choose to override default styles of semantic tags
- There are two types of lists: ordered `<ol>` and unordered `<ul>`
    - List elements contain list items `<li>`
    - Ordered lists create something like a numbered list
    - Unordered lists create something like a bulleted list
- Lists may be nested inside of lists
- `<em>` elements can emphasize key portions of text visually and as read aloud by a screen reader
- We can similarly convey importance with italics `<i>`, bold `<b>` and underline `<u>`

## HTML Advanced Text Formatting

- Description lists can be used to markup a set of terms and descriptions, such as Q&A or term/definition
    - `<dl>` element wraps the entire list
    - `<dt>` wraps each terms
    - `<dd>` wraps each definition
    - It is possible to give a single term multiple descriptions
- The `<blockquote>` element indicates that the enclosed content is a block quote, and HTML indents it by default
- The `<abbr>` element can be used with the `title` attribute to provide a fully elaborated version of an acronym or abbreviation
- The `<address>` element provides address/contact info, but should only be used to describe the document contained with the nearest `<body>` or `<article>` element (i.e. for the site author, and not for some random person talked about in the content)
- `<sub>` and `<super>` create subscript and superscript, respectively (i.e. for chemical formulas or mathematical exponents)
- When writing computer code:
    - `<pre>` preserves whitespace that would otherwise be ignored
    - `<var>` marks up variable names
    - `<kbd>` marks up keyboard input
    - `<samp>` marks up computer output
- `<time>` provides machine-readable alternatives to colloquially written dates and times in the content

## CSS

- We can apply CSS in three ways:
    1. Inline, with the style attribute in an HTML element
    2. In a `<style>` element within the `<head>` element
    3. In a .CSS file linked with the `<link>` element inside the `<head>` element
- Inline styles can be confusing and conflict with styles specified elsewhere. It is more difficult to maintain, and makes the HTML less readable as well.
> h2 {
    > color: black;
    > padding: 5px;
>}
- In the example above:
    - `h2` is the selector
    - `color` and `padding` are the declarations
    - `black` and `5px` are their respective properties

## Javascript (JS)

- Text enclosed in single quotation marks (i.e. `'this is a string'`) are strings
- Javascript operators include:
    - Arithmetic operators include:
        - `+` addition
        - `-` subtraction
        - `*` multiplication
        - `/` division
        - `**` exponentiation
        - `%` modulus
        - `++` increment
        - `--` decrement
    - Assignment operators assign a value to a variable. Examples include:
        - `=` x = y
        - `+=` same as `x = x + y`
        - `-=`, `*=`, `/=`, `**=`, `%=` function in the same pattern as `+=`
    - String operators operate on a string or strings. `+` concatenates, and `+=` functions similarly as in arithmetic
    - Comparison operators compare two variables and usual return a boolean value (true/false)
        - `==` equal to
        - `===` true equal (equal in value and type)
        - `!=` not equal
        - `>` greater than
        - `<` less than
        - `>=` greater than or equal to
        - `<=` less than or equal to
        - `?` evaluates an expression and executes one expression if truthy and a different expression if falsy
    - `&&` is logical `and` and evaluates to `true` if both operands are `true`, and `false` if one or more operands is `false`
    - `||` is logical `or` and evaluates to `true` if one or more operands is `true`, and `false` if both operands are `false`

- You can use functions to solve any number of real-world problems, such as implementing a scientific calculator inside of your website
- An `if` statement checks an expression, and if it evaluates to `true`, then the function will execute
    - An `else if` statement does the same thing, but only checks its expression if the first if statement evaluates to false
