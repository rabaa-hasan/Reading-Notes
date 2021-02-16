## Lists
### Ordered Lists
`<ol>`

The ordered list is created with the `<ol>` element.

`<li>`

Each item in the list is placed between an opening` <li> `tag and a closing `</li>`tag.



### Unordered Lists
`<ul>`

The unordered list is created with the `<ul>` element.

`<li>`

Each item in the list is placed between an opening` <li> `tag and a closing `</li>`tag.

example for ordered and unordered lists:

![ul](https://i.ytimg.com/vi/5tJBpZjMAbw/maxresdefault.jpg)

### Definition Lists
`<dl>`

The definition list is created with the `<dl>` element and usually consists of a series of terms and their definitions.

Inside the `<dl>` element you will usually see pairs of `<dt>` and `<dd>` elements.

`<dt>`

This is used to contain the term being defined (the definitionterm).

`<dd>`

This is used to contain the definition.

![dd](https://www.w3docs.com/uploads/media/default/0001/01/61895012b984c01394157fb224f371e8463d59bc.png)

### Nested Lists
You can put a second list inside an `<li>` element to create a sub- list or nested list.

![nastedList](https://images.slideplayer.com/25/7718725/slides/slide_4.jpg)

## Box Dimensions
### width, height
To set your own dimensions for a box you can use the height and width properties. The most popular ways to specify the size of a box are to use pixels, percentages, or ems.

```
div.box {
height: 300px;
width: 300px;
background-color: #bbbbaa;}
p {
height: 75%;
width: 75%;
background-color: #0088dd;}
```
Some page designs expand and shrink to fit the size of the user's screen. In such designs, the __min-width__ property specifies the smallest size a box can be displayed at when the browser window is narrow, and the __max-width__ property indicates the maximum width a box can stretch to when the browser window is wide.

```
td.description {
min-width: 450px;
max-width: 650px;
text-align: left;
padding: 5px;
margin: 0px;}
```
### Limiting Height
#### min-height, max-height
you might want to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the min-height and max-height properties.

```
p {
min-height: 10px;
max-height: 30px;}
```
### Overflowing Content
#### overflow
The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
* hidden : This property simply hides any extra content that does not fit in the box.
* scroll : This property adds a scrollbar to the box so that users can scroll to see the missing content.

### Every box has three available properties that can be adjusted to control its appearance:
1. Border
Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.
2. Margin
Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
3. Padding
Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

![box](https://codinglead.github.io/images/box-model.png)

### border-width
The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of the following values:
* thin
* medium
* thick

### border-style
You can control the style of a border using the border-style property.

 This property can take the following values:  __solid__ a single solid line dotted a series of square dots (if your border is 2px wide, then the dots are 2px squared with a 2px gap between each dot) 
 
 __dashed__ a series of short lines double two solid lines (the value of the border-width property creates the sum of the two lines) 

 __groove__ appears to be carved into the page
 
  __ridge__ appears to stick out from the page 
  
  __inset__ appears embedded into the page 

  __outset__ looks like it is coming out of the screen 
  
  __hidden / none__ no border is shown You can individually change the styles of different borders using:
```
border-top-style
border-left-style
border-right-style
border-bottom-style
```
### border-color
You can specify the color of a border using either RGB values, hex codes or CSS color names(as you saw on pages 251-252).

```
p.one {
border-color: #0088dd;}
```
### Shorthand
#### border
The border property allows you to specify the width, style and color of a border in one property (and the values should be coded in that specific order).
```
p {
width: 250px;
border: 3px dotted #0088dd;}
```
### padding
The padding property allows you to specify how much space should appear between the content of an element and its border.

You can specify different values for each side of a box using:
```
padding-top
padding-right
padding-bottom
padding-left
```
Or you can use a shorthand(where the values are in clockwise order: top, right, bottom, left):
`padding: 10px 5px 3px 1px;`

### Margin
The margin property controls the gap between boxes. Its value is commonly given in pixels, although you may also use percentages or ems.

You can specify values for each side of a box using:
```
margin-top
margin-right
margin-bottom
margin-left
```
You can also use the shorthand (where the values are in clockwise order: top, right, bottom, left):
`margin: 1px 2px 3px 4px;`

### Centering Content
If you want to center a box on the page (or center it inside the element that it sits in), you can set the left-margin and right-margin to auto.

### Change Inline/Block
#### display
The display property allows
you to turn an inline element
into a block-level element or vice
versa, and can also be used to
hide an element from the page.
The values this property can
take are:
* inline
This causes a block-level element to act like an inline element. block This causes an inline element to act like a block-level element.
* inline-block This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.
* none
This hides an element from the page. In this case, the element acts as though it is not on the page at all (although a user could still see the content of the box if they used the view source option in their browser).

### Hiding Boxes
#### visibility
The visibility property allows you to hide boxes from users but It leaves a space where the element would have been. This property can take two values:
* hidden: This hides the element.
* visible: This shows the element.

### Border Images
The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces.

### Box Shadows
The box-shadow property allows you to add a drop shadow around a box.
### Rounded Corners
#### border-radius
CSS3 introduces the ability tocreate rounded corners on any box, using a property called border-radius. The value indicates the size of the radius in pixels.

You can specify individual values for each corner of a box using:
```
border-top-right-radius
border-bottom-right-radius
border-bottom-left-radius
border-top-left-radius
```
You can also use a shorthand of these four properties (in clockwise order: top, right, bottom, left). For example:
`border-radius: 5px, 10px,
5px, 10px;`
### Elliptical Shapes
#### border-radius
To create more complex shapes, you can specify different distances for the horizontal and the vertical parts of the rounded corners. For example, this will create a radius that is wider than it is tall:
`border-radius: 80px 50px;  `

## ARRAYS
An array is a special type of variable. It doesn't just store one value; it stores a list of values.

You should consider using an array whenever you are working with a list or a set of values that are related to each other.

### CREATING AN ARRAY
You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array).
```
colors= ['white',
'black',
'custom'];
```
### VALUES IN ARRAYS
Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).

```
var col ors;
colors= ['whi te ' ,
'black ' ,
' custom '];

INDEX VALUE
o 'white '
1 'black'
2 'custom'
```
### ACCESSING & CHANGING VALUES IN AN ARRAY

![array](https://www.freecodecamp.org/news/content/images/2019/06/image-3.png)

### Conditional Statements
Very often when you write code, you want to perform different actions for different decisions.

You can use conditional statements in your code to do this.

In JavaScript we have the following conditional statements:

* Use if to specify a block of code to be executed, if a specified condition is true
* Use else to specify a block of code to be executed, if the same condition is false
* Use else if to specify a new condition to test, if the first condition is false
* Use switch to specify many alternative blocks of code to be executed

```
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}
```
### SWITCH STATEMENTS
A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

```
switch (level) {
case 'One ':
title= 'Level 1 ' ;
break;
case 'Two':
tit 1 e = ' Level 2 ' ;
break;
case ' Three' :
title = 'Level 3' ;
break ;
default :
title= 'Test';
break;
}
```
### The diffrence between If else and Switch
IF ... ELSE

* There is no need to provide an el se option. (You can just use an if statement.)
* With a series of if statements, they are all checked even if a match has been found (so it performs more slowly than switch).

SWITCH

* You have a default option that is run if none of the cases match.
* If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing better performance than multiple if statements).

If you use a data type JavaScript did not expect, it tries to make sense of the operation rather than report an error.

### JavaScript Loops
Loops are handy, if you want to run the same code over and over again, each time with a different value.
There are three types of loop: for, while, and do ... while. Each repeats a set of statements.

![loop](https://www.w3resource.com/w3r_images/java-for-loop-image1.png)

![looping](https://tutorial.techaltum.com/images/javascript-loops.jpg)
