# *Course 201, Entry 14: Documentation, Project Selection, & Team Workflow*

With the ability to change elements in form and over time, in such to be able to create animations, a lot is added to what a page can be. For any of the properties to be mentioned here, it is important to include vendor prefixes to maximize browser support. This means for each transform, transition, and animation property created, a copy for each vendor with its appropriate prefix attached should be created.

Prefixes:

-webkit-
-moz-
-o-

Example:

```
    -webkit-transition-property: background;
       -moz-transition-property: background;
         -o-transition-property: background;
            transition-property: background;
```

## CSS Transforms

The transform property has two major settings, 2D and 3D. Among these, there are different values.

2D Values:

+ Rotate (degrees)
+ Scale (Ratio of 1)
+ Translate (pixels and percentage)
+ Skew (degrees)
+ Perspective (pixels)
+ Transform-origin (pixels, percent, location side or corner)

Scale, Translate, and Skew can be X-axis, Y-axis, or combined comma-separated notation.

3D Values - All axes can be changed:

+ Rotate (degrees)
+ Scale (Ratio of 1)
+ Translate (pixels and percentage)

Another property for consideration when rotating on a 3D plane is *backface-visibility*. This property allows us to hide an object if it becomes fully turned around away from the screen.

### Use case

The variations offer a lot of capabilities. The various forms could allow for responsive tabs, links, and other navigations within a page, giving a page an interesting style.

## Transitions

To activate CSS styles for an element, the easiest way is to use pseudo-class elements, :hover, :focus, :active, and :target. Transitions are a morph, from one state to another.

Types of transitions:

+ transition-property
+ transition-duration
+ transition-timing-function
+ transition-delay

Using `transition` as shorthand, all of these can be combined into one, in order, separated by a space.

Here is a popular list of alterable properties which can be used in transition-property:

+ background-color
+ background-position
+ border-color
+ border-width
+ border-spacing
+ bottom
+ clip
+ color
+ crop
+ font-size
+ font-weight
+ height
+ left
+ letter-spacing
+ line-height
+ margin
+ max-height
+ max-width
+ min-height
+ min-width
+ opacity
+ outline-color
+ outline-offset
+ outline-width
+ padding
+ right
+ text-indent
+ text-shadow
+ top
+ vertical-align
+ visibility
+ width
+ word-spacing
+ z-index

Note, when listing multiple properties to alter, understand that the order is significant for other such properties such as transition-duration.

## Animations

Unlike transitions, animations allow for multiple changes, in keyframes.

To set an animation, the `@keyframes` selector can be used. Follow "@keyframes" with a unique name upon creation. Herein, the different keyframes can be set, at different percentages of animation. To call the animation property in another element, use the `animation-name` property, with the animation style name as the value.

Example:

```
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}
```

Here, "animation-iteration-count" sets if it is a loop, and "animation-direction" determines if it is a forwards and backwards loop.

The great advantage of CSS transitions on websites is how they increase engagement. Certainly, they are dazzling. This has a positive impression on visitors.

## Things I want to know more about

What kind of tools are out there which can make creating these transitions and animations easier and less manual? I can see these being very useful for any creation that I might come up with, offering some great effects to content.
