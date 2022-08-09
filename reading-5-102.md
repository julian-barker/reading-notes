[Home](README.md)

# Reading Assignment 5

## CSS

### What is CSS?

CSS stands for Cascading Style Sheet. Is is a format for applying style such as font, color, and complex layout to the structure and content of an HTML page.

### How do we include CSS in our pages?

CSS can be applied inline, internally, and externally. 
- Inline CSS is applied with the "style" attribute inside an HTML tag. 
- Internal CSS is applied in a \<style>\</style> tag  inside the HTML document. 
- External CSS is applied with a tag in the \<head> similar to this: 
    - \<link rel="stylesheet" href="style.css">.

Of note, inline CSS is applied with the highest priority, followed by internal/external CSS, and then whatever browser defaults may be present.

### Color

Color can be applied to fonts and backgrounds, and can be formatted in 4 ways:
- presets: predefined colors such as red, blue, green, black, coral, dark orange
- hexadecimal: a \# followed by six hex digits (0-f). ex. \#aaaaaa
- rgb: red, green, and blue values between 0 and 255. ex. rgb(0,155,30)
- hsl: hue (0-360), saturation (0-100%), lightness (0-100%). ex. hsl(120, 50%, 60%)
