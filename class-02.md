# Formating Text in HTML
## Headings
< h1>

< h2>

< h3>

< h4>

< h5>

< h6>

HTML has six "levels" of headings:

< h1> is used for main headings

< h2> is used for subheadings

![headings](https://www.schudio.com/wp-content/uploads/2016/10/html-headings.png?x97747)

## Paragraphs
< p>
To create a paragraph, surround the words that make up the paragraph with an opening < p> tag and closing < /p> tag.

## Bold & Italic
### Bold < b> 
By enclosing words in the tags < b> and < /b> we can make characters appear bold.

### Italic < i>
By enclosing words in the tags < i> and < /i> we can make characters appear italic.

## Superscript & Subscript
### Superscript< sup>
The < sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power.

![sup](https://www.wikitechy.com/step-by-step-html-tutorials/img/html-images/output-superscript-sup-tag-in-html.png)

### Subscript < sub>
The < sub> element is used to  contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.

![sub](https://www.wikitechy.com/step-by-step-html-tutorials/img/html-images/output-subscript-sub-tag-in-html.png)

## White Space
When the browser comes across two or more spaces next to each other, it only displays one space.
Similarly if it comes across a line break, it treats that as a single space too. This is known as __white space collapsing__.

## Line Breaks
< br />

As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag < br />.

## Horizontal Rules
To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the < hr /> tag.

![hr](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSGzfOtE57jAV1E8DaeyvV_lRXHKEG2jT5-FQ&usqp=CAU)

There are some text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages — they are known as __semantic markup__: 

### Strong < strong>
The use of the < strong>
element indicates that its
content has strong importance.

### Emphasis < em>
The < em> element indicates emphasis that subtly changes the meaning of a sentence.

## Quotations
There are two elements commonly used for marking up quotations:
### Blockquote < blockquote>
The < blockquote> element is used for longer quotes that take up an entire paragraph. Note how the < p> element is still used inside the < blockquote> element.

![blockquote](https://static.javatpoint.com/htmlpages/images/html-blockquote-tag2.png)

### < q>
The < q> element is used for shorter quotes that sit within a paragraph.

![q](https://www.w3docs.com/uploads/media/default/0001/01/c3cd8c0c415b5f193ccff281b49d67341462da0a.png)

## Abbreviations
< abbr> 
If you use an abbreviation or an acronym, then the < abbr>  element can be used. A title attribute on the opening tag is used to specify the full term.

![aabr](https://www.wikitechy.com/step-by-step-html-tutorials/img/html-images/output-abbreviation-tag-in-html.png)

## Citations < cite>
the < cite> element can be used to indicate where the citation is from.

![cite](https://codescracker.com/html/images/html-cite-work-title.jpg)

## Definitions < dfn>
in a document, it is known as the defining instance of it.

![dfn](https://www.wikitechy.com/step-by-step-html-tutorials/img/html-images/output-dfn-tag-in-html.png)

## Author Details
### < address>
The < address> element has quite a specific use: to contain contact details for the author of the page. It can contain a physical address, but it does not have to. For example, it may also contain a phone number or email address.
![address](https://www.w3docs.com/uploads/media/default/0001/01/7cac8939fb1c1d69f66d4d2d49f8e189536774b4.png)

## Changes to Content
### < ins>  < del>
The < ins> element can be used to show content that has been inserted into a document, while the < del> element can show text that has been deleted from it. 
 
![ins](https://static.javatpoint.com/htmlpages/images/html-del-tag2.png)

### < s>
The < s> element indicates something that is no longer accurate or relevant (but that should not be deleted).

![s](https://static.javatpoint.com/htmlpages/images/htmlstag.png)

# CSS
CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.


### CSS Associates Style rules with HTML elements

A CSS rule contains two parts: a selector and a declaration.

![element](https://lh3.googleusercontent.com/proxy/3eSEy3Gv3m4D4i-rBIR13lIv8ivyeGfsJbq49kg4Cab2MhiSs5fYlCwEWMVWWBzjz3IvkjrW0w3FxELFVm6lsfapPkRCo3Uz24SVkA)

Selectors indicate which element the rule applies to.
Declarations indicate how the elements referred to in the selector should be styled.

### CSS Properties Affect How Elements Are Displayed

CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon.

![pro](https://slideplayer.com/slide/13771255/85/images/9/CSS+PROPERTIES+AFFECT+HOW+ELEMENTS+ARE+DISPLAYED.jpg)

__Properties__ indicate the aspects of the element you want to change. For example, color, font, width, height and border.

__Values__ specify the settings you want to use for the chosen properties.

## Using External CSS
### < link>
The < link> element can be used in an HTML document to tell the browser where to find the CSS file used to style the page.

< link href="css/styles.css" type="text/css" rel="stylesheet" />

## Using Internal CSS
< style>
You can also include CSS rules within an HTML page by placing them inside a < style> element.


< style type="text/css">

body {

font-family: arial;

background-color: rgb(185,179,175);}

h1 {

color: rgb(255,255,255);}

< /style>

## Why use External Style Sheets?
External stylesheets allow you to completely separate your CSS from your HTML.

The benefits of using an external style sheet are:

* everything is stored within a single file.
* once changed/updated, the changes are reflected on all other pages that reference the stylesheet.
* this makes it easier to maintain larger websites.
* pages load quicker once the main CSS file has been cached.
* as a result bandwidth goes down.
* effectively, you’re able to change the entire look and feel of a website through a single file.

## Different versions of CSS & Browser Quirks
CSS1 was released in 1996 and 

CSS2 followed two years later.

Work onCSS3 has been ongoing but the major browsers have already started to implement it.

CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.

## color in CSS 
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

### rgb values
These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)

p {color: rgb(100,100,90);}

### hex codes
These are six-digit codes that represent the amount of red,green and blue in a color.

h2 {color: #ee3e80;}

### color names
There are 147 predefined color names that are recognized by browsers.
h1 {color: DarkCyan;}

## Background Color
background-color

the background-color property sets the color of the background for that box.

body {background-color: rgb (200,200,200);}

h1 {background-color: DarkCyan;}

## Understanding Color

Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.

The color of every pixel on the screen is expressed in terms of a mix of red, green, and blue — just like on a television screen.

![rgb](https://i1.wp.com/www.hisour.com/wp-content/uploads/2018/03/RGB-color-model.jpg?fit=720%2C720&ssl=1&w=640)

### Contrast
When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.

# JavaScript
## STATEMENTS
A script is a series of instructions that a computer can follow one-by-one.

Each individual instruction or step is known as a statement.

Statements should end with a semicolon.

## Comments 
You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.

## VARIABLE
A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

![var](https://tutorial.techaltum.com/images/js-variables.jpg)

## DATA TYPES
* NUMERIC DATA TYPE (0.75)
* STRING DATA TYPE ('H.
1 ' Ivy! 1)
* BOOLEAN DATA TYPE (true)

## USING A VARIABLE TO STORE A NUMBER

![img](data:image/png;base64,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)

## ARRAYS
An array is a special type of variable. It doesn't just store one value; it stores a list of values.

var colors;

colors ['white', 'black', ' custom'];

Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).

## EXPRESSIONS
1. EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE  (var color = 'beige';)
2. EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE  (var area = 3 * 2;)

## OPERATORS
Expressions rely on things called operators; they allow programmers to create a single value from one or more values.

* ASSIGNMENT OPERATORS Assign a value to a variable

color = 'beige';

* ARITHMETIC OPERATORS Perform basic math

area = 3 * 2;

* STRING OPERATORS Combine two strings 

greeting= 'Hi 1 + 'Mol ly';

* COMPARISON OPERATORS Compare two values and return true or false

buy = 3 > 5;

* LOGICAL OPERATORS
Combine expressions and return true or false

buy= (5 > 3) && (2 < 4);

## SWITCH STATEMENTS
A switch statement starts with a variable called the switch value.
Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

The purpose of the switch statement is to present the user with a different message depending on which level they are at. The message is stored in a variable called msg.

example:

switch (level) {

case 'One ':title= 'Level 1 ' ;
break;

case 'Two':title = ' Level 2 ' ;
break;

case ' Three' :title = 'Level 3' ;
break ;

default : title= 'Test';
break;
}
![switch](https://cdn.javascripttutorial.net/wp-content/uploads/2016/08/JavaScript-switch-case.png)
