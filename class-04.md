# HTML
## Links in HTML
Links are created using the `<a>` element. Users can click on anything between the opening `<a>` tag and the closing `</a>` tag. You specify which page you want to link to using the href attribute.

![links](https://lh3.googleusercontent.com/proxy/OUNscjCrL2dPUFLhzLpy8VtQQcw_k_NK-pHRRELysfXcPzSpZs4n0WrBNE_ii19A-KhvBlhEq_JNIRVsOub9HbRf__tHHefTzPPe7EZCj7RotoTdyOsXWsHl7-lO_RUIJU5ZTIV72_mMrJdqYhn6zC1vorb6B-P1FzNTnAz8)

### Linking to Other Sites
Links are created using the `<a>` element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.

When you link to a different website, the value of the href attribute will be the full web address for the site, which is known as an absolute URL.
An absolute URL starts with the domain name for that site, and can be followed by the path to a specific page. If no page is specified, the site will display the
homepage.

### Linking to Other Pages on the Same Site
When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a relative URL.

```
<p>
<ul>
<li><a href="index.html">Home</a></li>
<li><a href="about-us.html">About</a></li>
<li><a href="movies.html">Movies</a></li>
<li><a href="contact.html">Contact</a></li>
</ul>
</p>
```
### Directory Structure
On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.

![treeFiles](https://www.ixiasoft.com/documentation/IXIASOFT_CCMS/5.2/User_Guides_Advanced_User_DRM/per1389985984471.image)

Every page and every image on a website has a URL (or Uniform Resource Locator). The URL is made up of the domain name followed by the path to that page or image.

### Relative URLs
Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.

When you are linking to a page on your own website, you do not need to specify the domain name. You can use relative URLs which are a shorthand way to tell the browser where a page is in relation to the current page.

![relative vs live](https://i.pinimg.com/originals/b3/ac/b1/b3acb1896641896ab55c3e1c8e36eb73.png)

### Email Links

To create a link that starts up the user's email program and addresses an email to a specified email address, you use the `<a>` element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.

`<a href="mailto:jon@example.org">Email Jon</a>`

### Opening Links in a New Window
If you want a link to open in a new window, you can use the target attribute on the opening `<a>` tag. The value of this attribute should be  `_blank`.

`<a href="http://www.imdb com" target="_blank"> Internet Movie Database</a> `(opens in new window)

### Linking to a Specific Part of the Same Page

At the top of a long page you might want to add a list of contents that links to the corresponding sections lower down. Or you might want to add a link from part way down the page back to the top of it to save users from having to scroll back to the top.

```
<h1 id="top">Film-Making Terms</h1>
<a href="#arc_shot">Arc Shot</a><br />
<a href="#interlude">Interlude</a><br />
<a href="#prologue">Prologue</a><br /><br />
<h2 id="arc_shot">Arc Shot</h2>
<p>A shot in which the subject is photographed by an
encircling or moving camera</p>
<h2 id="interlude">Interlude</h2>
<p>A brief, intervening film scene or sequence, not
specifically tied to the plot, that appears
within a film</p>
<h2 id="prologue">Prologue</h2>
<p>A speech, preface, introduction, or brief scene
preceding the the main action or plot of a film;
contrast to epilogue</p>
<p><a href="#top">Top</a></p>
```

### Linking to a Specific Part of Another Page
the href attribute will contain the address for the page (either an absolute URL or a relative URL), followed by the `#` symbol, followed by the value of the id attribute that is used on the element you are linking to.

For example, to link to the bottom of the homepage of the website that accompanies this book, you would write:

`<a href="http:/www. htmlandcssbookcom/ #bottom">`

# CSS
## Key Concepts in Positioning Elements
### Building Blocks

CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

Block-level elements start on a new line Examples include:

`<h1> <p> <ul> <li>`

Inline elements flow in between surrounding text Examples include:

`<img> <b> <i>`

### Containing Elements
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element.

![contaiener](https://i.stack.imgur.com/iejBS.png)

### Controlling the Position of Elements

CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.

#### Normal Flow
![normalFlow](https://image.slidesharecdn.com/css-160124050959/95/css-79-638.jpg?cb=1453612252)

#### Relative Positioning
#### Absolute positioning

![ab](https://i.stack.imgur.com/wA8sA.gif)

### you can include multiple CSS Files in one Page.

# JavaScript
## Function
Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

```
var msg = 'Sign up to receive our newsletter for 10% off!';
function updateMessage() {
var el = document.getElementByld('message'};
el .textContent = msg;
}
updateMessage(};
```
This statements are not run until the function is called. The function is only called on the last line of this script.

![fun](https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/declaration.svg)

### The JavaScript call() Method
```
var person = {
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}
var person1 = {
  firstName:"John",
  lastName: "Doe"
}
var person2 = {
  firstName:"Mary",
  lastName: "Doe"
}
person.fullName.call(person1);  // Will return "John Doe"
```

Expressions produce a value. They can be used where values are expected. If a function is placed where a browser expects to see an expression, (e.g., as an argument to a function), then it gets treated as an expression.

### IMMEDIATELY INVOKED FUNCTION EXPRESSIONS
This way of writing a function is used in several different situations. Often functions are used to ensure that the variable names do not conflict with each other (especially if the page uses more than one script).

### VARIABLE SCOPE
The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.
#### LOCAL VARIABLES
When a variable is created inside a function using the var keyword, it can only be used in that function. It is called a local variable or function-level variable.

#### GLOBAL VARIABLES
If you create a variable outside of a function, then it can be used anywhere within the script. It is called a global variable and has global scope. In the example shown, wa 11 Size is a global variable.

### HOW MEMORY & VARIABLES WORK
Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed.

### CREATING THE VARIABLES IN CODE
Each variable that you declare takes up memory.


```
var wi dth = 15;
var height = 30;
var isWal l = true;
var canPaint = true;
```

### NAMING COLLISIONS
You might think you would avoid naming collisions; after all you know which variables you are using.

```
II Show size of the building plot
function showPlotSize(){
var width = 3;
var height = 2;
return 'Area: " + (width* height);
var msg = showArea()
```

## 6 Reasons for Pair Programming
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness
