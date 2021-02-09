# CSS 
CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
X Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
Declarations are made up of two parts: the properties of the element that you want to change, and the values
of those properties.
 For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
CSS rules usually appear in a separate document,although they may appear within an HTML page.

## Colors in CSS
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
* rgb values 

p {
color: rgb(100,100,90);}

* hex codes

h2 {
color: #ee3e80;}

* color names

h1 {
color: DarkCyan;}

## Background Color
background-color

CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.
You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values,hex codes, and color names(covered on the next page).

body{background-color:rgb(200,200,200);}

## Understanding Color
Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.
Computer monitors are made up of thousands of tiny squares called pixels (if you look very closely at your monitor you should be able to see them). When the screen is not turned on, it's black because it's not emitting any light. When it's on, each pixel can be a different color, creating a picture.
The color of every pixel on the screen is expressed in terms of a mix of red, green, and blue — just like on a television screen.
![rgb](https://i1.wp.com/www.hisour.com/wp-content/uploads/2018/03/RGB-color-model.jpg?fit=720%2C720&ssl=1&w=640)

### RGB Values
Values for red, green, and blue
are expressed as numbers
between 0 and 255.

rgb(102,205,170)

This color is made up of the following values:
102 red
205 green
170 blue

### Hex Codes

Hex values represent values
for red, green, and blue in
hexadecimal code.

#66cdaa

The value of the red, 102, is expressed as 66 in  hexadecimal code. The 205 of the green is expressed as cd and the 170 of the blue equates to aa.

### Color Names

Colors are represented by
predefined names. However,
they are very limited in number.


## Contrast

When picking foreground and background
colors, it is important to ensure that there is
enough contrast for the text to be legible.

### CSS3: Opacity
opacity, rgba

CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements.
The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).
The CSS3 rgba property allows you to specify a color.

p.one {
background-color: rgb(0,0,0);
opacity: 0.5;}

p.two {
background-color: rgb(0,0,0);
background-color: rgba(0,0,0,0.5);}

CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values.

CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.
