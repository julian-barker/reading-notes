[Home](../README.md)

# Class 11

## Audio and Video

- Early in the web's life, video and audio were not natively supported by HTML, and were embeddedthrough software solutions like Flash, which had security issues. HTML now has native support with the `<audio>` and `<video>` tags.
- The `<video>` tag is used to embed video into a page.
  - `src` works the same as in the `<img>` tag and specifies the location for the browser to find the video.
  - `controls` is an attribute with no value that tells the browser to implement its own native form of video controls. If you wish to specify your own format, it must at least include stop/play, and volume control functionality.

- The text inside the video tag is fallback content, which is similar to the alt attribute in an image. Often it is used to provide a hyperlink to the source of the video.
- Formats like MP3, MP4, and WebM are container formats. They describe how the audio/video tracks, metadata, and text/subtitles are stored.
- Not all browsers support all audio/video formats and container formats, so it is a good idea to provide multiple sources.
  - A WebM container typically packages Vorbis or Opus audio with VP8/VP9 video. This is supported in all modern browsers, though older versions may not work.
  - An MP4 container often packages AAC or MP3 audio with H.264 video. This is also supported in all modern browsers, as well as Internet Explorer.
  - The Ogg container tends to use Vorbis audio and Theora video. This is best supported in Firefox and Chrome, but has basically been superseded by the better quality WebM format.

> An "MP3 file" is actually an MPEG-1 Audio Layer III (MP3) audio track stored within an MPEG or MPEG-2 container. This is especially interesting since while most browsers don't support using MPEG media in the `<video>` and `<audio>` elements, they may still support MP3 due to its popularity.

> Note: Several popular formats, such as MP3 and MP4/H.264, are excellent but are encumbered by patents; that is, there are patents covering some or all of the technology that they're based upon. In the United States, patents covered MP3 until 2017, and H.264 is encumbered by patents through at least 2027.

>Because of those patents, browsers that wish to implement support for those codecs must pay typically enormous license fees. In addition, some people prefer to avoid restricted software and prefer to use only open formats. Due to these legal and preferential reasons, web developers find themselves having to support multiple formats to capture their entire audience. --MDN Web Docs

- to provide multiple formats for a/v, we can take the source attribut out of the a/v tag and place it in the content as its own tag, like so:

``` HTML
<video controls>
  <source src="some link" type="video/mp4">
  <source src="some other link" type="video/webm">
  <p>The video could not load. Here is a <a href="some link">link to the video</a> instead.</p>
</video>
```

- The `type` attribute is not strictly required, but is strongly recommended.
- Additional `<video>` attributes are below:
  - `width` and `height` control the respective attributes. You can also control these with CSS.
  - `autoplay` makes the audio or video play as soon as it loads. This is annoying and ill-advised in most cases.
  - `loop` makes the audio or video start playing again as soon as it finishes.
  - `muted` causes the video to be muted at the start.
  - `poster` is the image displayed before the video plays.
  - `preload` determines if the video buffers the media file (`auto`), the metadata (`metadata`), or none (`none`).

- The `<audio>` tag is similar to the its video counterpart, save for a few differences:
  - It does not take up significant space on the screen. Because of this, it supports neither the `width`/`height` attributes, nor the `poster` attribute.

- We use WebVTT eith the `<track>` element to provide cues such as timed descriptions, subtitles, and captions.
- `<track>` should be placed after all `<source>` elements, and should link to a .vtt file with the `src` attribute. The `kind` attribute specifies if it is captions, subtitles, or timed descriptions. `srclang` tells the browser what language the subs are in. `label` helps readers find the language they are looking for.

- Example:

```HTML 
<track kind="subtitles" src="subtitles_es.vtt" srclang="es" label="Spanish">
```

## CSS Grid

- CSS Grid is a powerful CSS module that, in contrast with Flex, allows us to arrang items in two dimensions instead of one.
- It is used with `display: grid` on a parent container, similar to Flex
- `inline-grid` creates an inline-level grid
- A grid-line is a vertical or horizontal line used to define the cells in between.
- A grid cell is the space between two adjacent vertical grid lines and two adjacent horizontal lines.
- A grid track is the space between two adjacent gridlines, spanning the entire height or width of the grid.
- A grid area is the space surrounded by four grid lines, and can be composed of any number of cells
- A grid item's location is determined by `grid-column-start`, `grid-column-end`, `grid-row-start`, and `grid-row-end`. It can also be defined by start values and the number of rows and/or columns spanned.
- Grid sizes are defined by `grid-template-columns` and `grid-template-rows`.
- Grid lines can have multiple names, defined at the definition of the grid. They also have default names given based on assignment of `grid-template-areas`.
- `grid-areas` are used to give an item a name to be referenced by the `grid-template-areas` property.
- `grid-template` is a shorthand property to define `grid-template-rows`, `grid-template-columns`, and `grid-template-areas`.
- Example syntax below:

```CSS
.container {
  grid-template:
    [row1-start] "header header header" 25px [row1-end]
    [row2-start] "footer footer footer" 25px [row2-end]
    / auto 50px auto;
}
```

- `row-gap` and `column-gap` are used to specify the width of grid lines, or the width of "gutters". Of note, these gutters only manifest between cells, and not on the outer borders of the grid.
- `gap` is a shorthand for `row-gap` and `column-gap`
- `justify-items` aligns items on the row-axis, whereas `align-items` aligns them on the column axis.  Accepted values are `start`, `end`, `center`, and `stretch`.
  - can also be used on grid-items via `justify-self` and `align-self`.
  - `place-items` is shorthand to define both.

- `justify-content` and `align-content` lay out the grid within its grid container, if it does not fill its container.
  - Accepted values are `start`, `end`, `center`, `stretch`, `space-between`, `space-around`, `space-evenly`.

- `grid-auto-rows` and `grid-auto-columns` define the size of rows/columns outside of the explicit grid. (defined at grid definition)
- `grid-auto-flow` says what to do with items not explicitly placed on the grid.
  - `row` tells the algo to fill rows in turn, adding new ones as necessary
  - `columns` does the same, with respect to columns
  - `dense` attempts to fill any existing holes in the grid when items small enough come up (only changes visual order, so it could negatively impact accessibility)

- `grid` is a shorthand to specify all above properties.
- `fr` is fractional units and refers to a portion of the free space after explicit sizes are given. Ex. 1fr 1fr 1fr 60px would give the right-most column 60px width, and the first three columns would evenly divide the remaining space on the left.
- `minmax()` sets a min and max for the length, which is useful in combo with fr units, if you only want columns to be able to shrink so far.
- `repeat()` takes a number and a size, and equates to that number amount of columns or rows of that size.
- `display: contents` can be given to a grid-item to plae child elements on the same grid as the parent, similar to subgrids (which are currently only supported in firefox)

## Responsive Images

- Responsive images are images that work well on screens of differing sizes.
- Responsive images can improve the site by providing a better viewing experience for users, by not having adverse affects on the layout or visibility of other elements, and by consesrving user bandwidth when possible.
- `srcset` is used in conjunction with `src` to specify multiple images to use for different scenarios. It takes its images' intrinsic widths ( in `w`, not `px`)
- `sizes` provides the various sizes to dislpay the different images at. It is used in conjunction with a media condition, ie `(max-width: 600px) 480px` meaning that on screen sizes of 600px and smaller, display the corresponding image at 480px.
- `srcset` is helpful because images are loaded before any CSS or javascript, meaning you could not use javascript to immediately read the image, gather its size, and change it appropriately. `srcset` allows this
- `<picture>` is used with `<source>` tags for art direction to provide different images for different sizes. You must provide an `<img>` right before the `</picture>`, as a default.
