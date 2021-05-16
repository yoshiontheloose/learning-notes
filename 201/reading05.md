***Duckett HTML Book***

# Chapter 5: Images (p 94-125)

_Good Practice_: Make a folder (and sub-folders if necessary) for all of the images used on your site.

`<img>` - add an image to the page. No closing tag. Needs the following attributes:

- `src` -tells browser where to find image file
- `alt` - text description of the image. For screen reader software.  
_Optional_: title - additional info about the image

`height` and `width` - specify in pixels

Where to place:

- Before a paragraph
- Inside the start of a paragraph
- Middle of a paragraph

Rules for creating images:

- Save images in correct format
- Save images in the right size
- measure images in pixels

Use .jpeg for colorful immages and GIF or .png for images with few colors/large amount of the same color

Vector Images

- Dimensions can be increased without affecting the quality/resolution
- current method of using vector images on websites involves saving a bitmap version of the original and using that
- SVG: scalabel vector graphics - new format to display vectors directly onto the web.

Trasparent images (p118)

`<figure>` (needs closing tag) - contains images and their caption together. Can contain multiple images.

`<figcaption>` (closing tag) - caption for the image

---
# Chapter 11: Color (p 246-263) CSS

*que everything about color from high school art*

Color property by iteself changes text color

Ways to specify color:

- RGB values (0, 0, 0)
- RGBA values - Adds opacity (0, 0, 0, 0)
- Hex codes #66cdaa
- Color names

HSL colors - Hue, saturation, Lightness

- background-color: hsl(0, 0%, 0%)

HSLA - adds Alpha for transparency. from 0 to 1.0

- background-color: hsla(0, 0%, 0%, 0.5)

---

# Chapter 12: Text (p 264-299)

Typeface will only display if it's installed on the user's computer

Font Stack - order of typeface preference

PCs render type less smoothly, Mac users should check what it looks like on PC

`font-family` - can list more than one in case user doesn't have a typeface installed  
`font-size` - measured in pixels or percentages  
`@font-face` - use a font even if not installed on user's computer

- add font to style sheet.
```
@font-face {
  font-family: 'ChunkFiveRegular';
  src: url('fonts/chunkfive.eot');}

h1, h2 {
  font-family: ChunkFiveRegular, Georgia
}
```

`font-weight` - normal or bold  
`font-style` - normal, italic, or oblique  
`text-transform` - uppercase, lowercase, or capitalize  
`text-decoration` - none, underline, overline, line-through, blink  
`line height` - space between text. Descender and ascender, lowest point and highest point  
`letter-spacing` - "kerning" typographer term for soace between each letter  
`word-spacing`
`text-align` - left, right, center, justify

- justify - every letter in a paragraph except the last line will take up the full width of the containing box

`vertical-align` - similar to HTML align attribute. Used with inline elements `<img>` `<em>` or `<strong>`

- Values: baseline, sub, super, top, text-top, middle, bottom, and text-bottom. (p 286)

`text-indent` - indents first line of text in an element. measured in pixels

`text-shadow` - four values: shadow to left or right, top or bottom distance, blur amount (optional), color of drop shadow

## Pseudo-elements

`:first-letter`, `first-line` - specify different values to text

`:link`, `:visited` - styles for unvisited or visited links.  
`:hover` - hovering with mouse  
`:active` - button being clicked  
`:focus` - when you select an input box or hover a mouse over it  

**Attribute Selectors** (p 292) - allow you to create rules applied to elements with an attribute of a specific value 

---
"Reference for a TLDR" - https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d



[<<<Back](README.md)