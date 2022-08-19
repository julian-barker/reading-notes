[Home](../README.md)

# Class 05

## HTML Media

1. A real world example for the usefulness of the alt attribute is that it displays when the image fails to load, so it will still convey some information to the user about what should have been displayed.
2. The alt tag can also improve accessibility, as well as having captions for images.
3. A figure image is useful in that it is semantic and links a caption to its image, as opposed to just a line of text nested with an image in a `<div>`
4. Images are made up with pixels. A gif (raster) image says exactly what should be in each pixel of the image. An svg (vector) image starts with a blank canvas and provides instructions for how to draw the various shapes and colors that comprise an image.
5. To display a screenshot, you would use a gif (raster), because you want to specify each pixel, and the screenshot cannot be easily described as a combination of shapes/functions.

## CSS Colors and Styling HTML

1. Background colors are exactly what you would expect, whereas foreground color is everything on top of that. This normally just refers to the text, but it applies also to things like underlines.
2. To give a colorless blog some character, I met set a background color for the entire site, and then a different background color for high level elements like the header, main, and footer. I might set a funky color for the heading as well.
3. When choosing fonts, you should consider the color in contrast with the background, as well as the size of the font, and whether you want a serif or sans-serif font for style/readability.
4. Font properties:
  - `font-size` changes the size of the font. It can be specified in a number of ways, including in pixels and in reference to the browsers base font size.
  - `font-weight` changes how thick the strokes of the letters are. This is where you could text bold, but you can be more specific than just bold or not bold
  - `font-style` adds other styling such as italics
5. To change the character spacing, you could use a specific font-family, such as monospace, or the `text-transform: full-width` property.
