# *Course 201, Entry 7: Object-Oriented Programming, HTML Tables*

## Domain Modeling

why we need domain modeling.

A domain model creates a conceptual framework for a feature. This serves well when communicating between business folks and programming management.

1. When creating a model with multiple instances, create a single object which will hold a constructor function. This constructor function is what will hold the  properties.

2. Methods will then be created with each doing a singluar task. Within these different methods, `this` can be used to access the objects properties and other methods.

3. Instances can then be created using the `new` keyword, followed by a call to the constructor function, all stored within a variable.

## Tables

Tables are great when implemented correclty. However, tables should not be used for layouts. The reasons are:

+ Poor accessibility for screen readers.
+ There ends up being a lot more code than necessary.
+ Table so easy to create with responsiveness to various screen sizes.

### Semantic Elements

Some table semantic elements include: 

+ `<th>` - Table header
+ `<td>` - Table data
+ `<tr>` - Table row
+ `<colspan>` - Number of columns
+ `<rowspan>` - Number of rows
+ `<colgroups>` - Holds the `<col>` elements
+ `<col />` - Allows for CSS formatting to columns


## Constructors

What is a constructor and what are some advantages to using it?

### this - Object Literal vs Constructor

How does the term this differ when used in an object literal versus when used in a constructor?

### Prototypes

Explain prototypes and inheritance via an analogy from your previous work experience.
NOTE: This is a very common front end developer interview question


## Things I want to know more about
