***Duckett HTML Book***

# Chapter 15: “Layout” (p 358-404)

CSS treats each HTML element as if it's in it's own box.

- **Block level element**: Starts on a new line. Main building blocks of a layout.
  * Ex: `<h1> <p> <ul> <li>`
  
- **Inline element**: Flow between surrounding text.
  * Ex: `<img> <b> <i>`

- **Containing element/parent element**: A block level element containing other block level elements.
  * Ex: `<div> <body>`

### Positioning

Specify positioning scheme in css by using `position:` property.  

*(Think of the image on Word with the dog)*

**Normal Flow** - Default. Straight. Does not need to be specified. (`position: static` if it did. 

**Relative Positioning** - Shifted with TRBL offset properties. Does not affect position of surrounding elements.

**Absolute Positioning** - Taken out of normal flow. Moves with the scroller. Does not affect surrounding elements.

**Fixed Positioning** - Form of absolute positioning. positions in relations to the browswer window. Uses TRBL offset properties. 

**Floating Elements** - Far left or right of a containing box. Becomes a block level element. Text flows around it. 

_Use the "width" property for how wide the floated element should be!_

  - Commonly used to float boxes next to each other. Height of box can affect where the element sits.
  - `clear:` - says that no element in the same containing box should touch the left or right sides.
    *left, right, both, none

**z-index** - "stacking content." Used if boxes overlap. Similar to "bring to front" and "send to back."

Creating multi-column layouts with floats:

- use a `<div>` element to represent each column. Can be nested. `<div class="column1of2">`
- Width - sets width of columns
- Float - positions columns next to each other
- margin - makes a gap between columns

**Standard page size - 960-1000 pixels wide**
Top 600 pixels to tell what site is about. 

**Fixed Width Layouts**  
Measurements in pixels. Size stays the same.

**Liquid Layouts**  
Measurements in percentages. Size stretches or shrinks.

Grids help structure the page.  

-----
# Lecture Notes 
Source: [https://github.com/codefellows/seattle-code-201d75/blob/main/class-08/lectureNotes.md]

## Alternative Options for Layouts
- previously we moostly had float
  - pros: lets us move things out of flow
  - cons: not super precise, it can mess up other things on your page, that you then have to fix and put back in flow
- positioning with absolute relative
  - cons: a bit involved
  - pro: allows you to visually place items on top of other items

- new options
  - flexbox
    - simple way to divide and align boxes
    - https://css-tricks.com/snippets/css/a-guide-to-flexbox/
  - grid
    - a grid system that allows you to position elements to grid squares
    - https://css-tricks.com/snippets/css/complete-guide-grid/