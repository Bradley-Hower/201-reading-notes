# *Course 201, Entry 8: CSS Layout*

## Flexbox

### One-dimensional

When flexbox `flex-wrap`  is set to `wrap`, it will create new **flex lines** for the content items (when set to "nowrap" - as by default, the content will overflow). Flex lines are independent of other flex lines. This demonstrates itself in alignment. Alignment is applied independently. Thus the an item on line two can not be set to align with an item on line one. This is what is meant when it is said that flexbox is one-dimensional. Only one axis can be controlled. Either horizontally or vertically. Horizontially is within a line, vertically is between lines.

These two axis have two names. The **main axis** and the **cross axis**. The main is left to write content placement. Cross axis is top to bottom content placement. However, this is dependent on set writing directions which are language dependent.

### Direction

The dircetion of content can be overridden with the following values for `flex-direction`:

+ row
+ row-reverse
+ column
+ column-reverse

Thus, main axis content can be place vertically, but still use justify for the alignment. See alignment further down.

### Content Spacing

Content can be spaced from three primary properties, `flex-grow`, `flex-shrink`, and `flex-basis`. 

Grow - Enlargement of items on expansion of window.
Shrink - Shrink of items on contrasion of window.
Basis - On auto, sets content sizes to where they all fit and match. Alternatively, size can be set.

And while these each can be custom modified, it makes more sense to use the encompassing property `flex` to select each of these to a preset. Moreover, using `flex` passes these properties to children elements. 

The value options are:

+ initial - Grow: no. Shrink: yes. Basis: auto.
+ auto - Grow: yes. Shrink: yes. Basis: auto.
+ 1 - Grow: yes. Shrink: yes. Basis: no.
+ none - Grow: no. Shrink: no. Basis: no.

### Alignment

There are two main categories of properties for alignment:

justify-... - main axis
align-... - cross axis

The next subcategories for these are to which they apply:

...-self - this element
...-items - this element and all of its children

The values that can be attached to these are:

+ stretch - content fills its flex line space.
+ flex-start - pushes item to start of the axis.
+ flex-end - pushes items to the end of the axis.
+ center - aligns all items to the middle center.

### Space

Space along the main and cross access can be set with the shorthand `place-content`. The first value is for the main axis, the second value is for the cross axis.

The values that can be attached to these are:

+ space-around - puts an even amount of space between items, and half space on the far ends.
+ space-between - puts an even amount of space between items, no space on the far ends.
+ space-evenly - puts an even amount of space between items and on the far ends.

### Accessibility

While flexbox has many capabilities for modification, accssibility should be kept in mind. Screen readers will work according to the DOM, in other words, how the HTML is set up. So while content order and alignment can be changed, one should keep in mind the effects for accessibility. If content flow is different from the HTML, then change the HTML. For this reason, the `order` property should be avoided.

## Things I want to Know more About