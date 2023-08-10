# *Course 201, Entry 3: HTML Lists, Control Flow with JS, and the CSS Box Model*

## HTML - Lists

Lists in HTML give some organization to a page. How though can we maximize the use? What are some feature tweaks?

## Using Unordered Lists

Unordered lists are great for putting down a list of items in no particular order. How does one know if it is applicable? Trying changing the order. If the list still makes logical sense, then an unordered list should work fine.

## Using Ordered Lists

Conversely, if you change the order of a list and the piece becomes non-sensicle, then an ordered list is best. Some things are inherintly ordered, such as listing out a process, procedures, steps, instructions, directions, and other things of the list. When precision matters, an ordered list is probably best.

## Changing the bullet style of unordered list items

To change the bullet style, the attribute `type` can be added to an enclosed list item. The different attribute types for "type are as follows:

+ `a` lowercase leters
+ `A` uppercase letters
+ `i` lowercase Roman numerals
+ `I` uppercase Roman numerals
+ `1` for numbers, the default

## Two ways to change list item numbers

The first way that the numbers in an ordered list can be changed is by entering the attribute `reveresed`. This will reorder the list in decending order. 

The second way that list numbers can be changed is by starting off with a different number. Using the `start` attribute, the list can be started at any specified number. 

## CSS - The Box Model

The box model in CSS allows one to understand how the properties padding, margin, and border are set. With this understanding, proper sizing can be set.

### The Roles of  Margin and Padding

Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

If margin and padding were in a story, the plot would be starred by padding. Padding is what we see, it is how we understand the characters which are the elements. We see their colors, styles sizes, etc. and assume it's just them. However, margin is what sets the tone. It is the boss, leader, orator of the story. Margins say where the limits are, where absoultely, padding can not go.

### Four Parts of an HTML Elements Box

The four parts of the an HTML element box:

+ Content box - This is where the goods are. Text, video, pictures, games, all exist here.
    Sizing options: inline-size, block-size, or width and height.
+ Padding box - This is the filling outside of the content. Any background color will fill here. Likeunto the "mat" of a picture frame.
+ Border box - This gives the edge to content, like a frame to a painting.
+ Margin box - This is the white space, or airgap, to other content elements.

By default, under the standard box model, all sizing is added on top of the conent. Width and height are set there.

Under the alternative box model, height and width are set to the total outside, then any padding, margin and borders are set there within. Outwards in, rather than inwards out. ALterntive sizing can be set by adding the following declaration to the CSS. `box-sizing: border-box`

## JS - Arrays, Operators, Expressions, Conditionals, and Loops

### Arrays

What data types can you store inside of an Array?
Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

Example:

 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];




### Operators

List five shorthand operators for assignment in javascript and describe what they do.
Read the code below and evaluate the last expression and explain what the result would be and why.

Example: 

 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;




### Conditional Statements

Describe a real world example of when a conditional statement should be used in a JavaScript program.




### Loops

Give an example of when a Loop is useful in JavaScript.



