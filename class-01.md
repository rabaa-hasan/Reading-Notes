# Introductory HTML and JavaScript
## How Pages Use Structure in HTML
Any website, and you could break down the site into remarkably predictable sections. Developers write HTML in a way that permits consistent content structure across the entire web. This reduces cognitive work for users and makes different sites display reliably across browsers, screen readers, and search engines.

![webPageStructure](https://i.pinimg.com/originals/46/e2/1c/46e21c46e7001fca6554cd45562268fa.jpg)
Think about the stories you read in a newspaper: for each story, there will be a headline, some text, and possibly some images. If the article is a long piece, there may be subheadings that split the story into separate sections or quotes from those involved. Structure helps readers understand the stories in the newspaper.

Now think about a very different type of document — an insurance form. Insurance forms often have headings for different sections, and each section contains a list of questions with areas for you to fill in details or checkboxes to tick. Again,the structure is very similar online.

## Structuring Word Documents
### Headings
The use of headings and subheadings in any document often reflects a hierarchy of information. For example, a document might start with a large heading, followed by an introduction or the most important information.
#### How to Add Headings Using HTML
The following are best practices for using HTML headings:

Use < h1> for the main heading of the page. For most pages, there will be only one < h1>.

Use < h2> for subheadings beneath the main heading.

Use additional levels of headings (< h3> through < h6>) as needed if there are additional levels of sub-headings within your web page content.

![headings](https://www.schudio.com/wp-content/uploads/2016/10/html-headings.png?x97747)

### Lists
Lists can provide additional information such as the number of items in the list. This is extremely helpful information for users 

All document authoring environments include features that enable you to add bulleted lists or numbered lists.
### Tables
Tables should be used only for presenting rows and columns of data, not for organizing the layout of the page. 
### Forms 
Most forms include form fields accompanied by labels or prompts. In order to figure out which labels accompany which fields.
## HTML Describes the Structure of Pages
To describe the structure of a web page, we add code to the words we want to appear on the page. You can see the HTML code for this page below.

< html>

< body>

< h1>This is the Main Heading< /h1>

< p>This text might be an introduction to the rest of
the page. And if the page is a long one it might
be split up into several sub-headings.
< /p>

< h2>This is a Sub-Heading< /h2>

< p>Many long articles have sub-headings so to help
you follow the structure of what is being written.
There may even be sub-sub-headings (or lower-level
headings).< /p>

< h2>Another Sub-Heading< /h2> 


< p>Here you can see another sub-heading.< /p>


< /body>

< /html>

### HTML Uses Elements to Describe the Structure of Pages
Elements are usually made up of two tags: an opening tag and a closing tag. (The closing tag has an extra forward slash in it.)  Each HTML element tells the browser something about the information that sits between its opening and closing tags.
#### Tags
![tags](https://clearlydecoded.com/assets/images/posts/2017-09-04-anatomy-of-html-tag/simple-p-tag.png) 

#### Attributes Tell Us More About Elements
They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign.

![attribute](https://clearlydecoded.com/assets/images/posts/2017-09-04-anatomy-of-html-tag/html-tag-attributes.png)

## Body, Head & Title
### Body
< body>

Everything inside this element is shown inside the main browser window.
### Head
< head>

Before the < body> element you will often see a < head> element. This contains information about the page (rather than information that is shown within the main part of the browser window that is highlighted in blue on the opposite page). You will usually find a < title> element inside the < head>element.
### Title
< title>

The contents of the < title> element are either shown in the top of the browser, above where you usually type in the URL of the page you want to visit.
## Looking at How Other sites are Built
When the web was first taking off, one of the most common ways to learn about HTML and discover new tips and techniques was to look at the source code that made up web pages.
Once you have opened the page, you can look for the View menu in your browser, and select the option that says __Source__ or __View source__. (The title changes depending on what browser you
are using.)
## Extra Markup
### DOCTYPEs
Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using.
+ HTML5 < !DOCTYPE html>
+ HTML 4 < !DOCTYPE html PUBLIC
"-//W3C//DTD HTML 4.01 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">
+ Transitional XHTML 1.0 < !DOCTYPE html PUBLIC
"-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/
xhtml1-transitional.dtd">
+ Strict XHTML 1.0  < !DOCTYPE html PUBLIC
"-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/
xhtml1-strict.dtd">
+ XML Declaration   < ?xml version="1.0" ?>

### Comments in HTML
< !-- --> 

If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:

< !-- comment goes here -->

### ID Attribute
Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore.

example:

< p id="pullquote">Every time I view the sea I feel a calming sense of security, as if visiting my ancestral home; I embark on a voyage of seeing.
< /p>
### Class Attribute
Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page.

The class attribute on any element can share the same value.

example:
< p class="important">For a one-year period from November 2010, the Marugame Genichiro-Inokuma Museum of Contemporary Art (MIMOCA) will host a cycle of four Hiroshi Sugimoto exhibitions.< /p>

### Block Elements
Some elements will always appear to start on a new line in the browser window. These are known as block level elements.
Examples of block elements are:

< h1>, < p>, < ul>, and < li>.

### Inline Elements
Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements.
Examples of inline elements are:

< a>, < b>, < em>, and < img>.

### Grouping Text & Elements In a Block
#### < div>
The < div> element allows you to group a set of elements together in one block-level box.

< div id="header">

< img src="images/logo.gif" alt="Anish Kapoor" />

< ul>

< li>< a href="index.html">Home< /a>< /li>

< li>< a href="biography.html">Biography< /a>< /li>

< li>< a href="works.html">Works < /a>< /li>

< li>< a href="contact.html">Contact< /a>< /li>

< /ul>

< /div>< !-- end of header -->

### Grouping Text & Elements Inline
#### < span>
The < span> element acts like an inline equivalent of the < div> element. It is used to either:

1. Contain a section of text where there is no other suitable element to differentiate it from its surrounding text
2. Contain a number of inline elements.

exmple:

< p>Anish Kapoor won the Turner Prize in 1991 and exhibited at the < span class="gallery">Tate Modern< /span> gallery in London in 2003.< /p>

### IFrames
< iframe>

An iframe is like a little window that has been cut into your page — and in that window you can see another page. The term iframe is an abbreviation of inline frame.

example:

< iframe

width="450"

height="350"

src="http://maps.google.co.uk/maps?q=moma+new+york
&amp;output=embed">

< /iframe>

### Meta

The < meta> tag allows you to supply all kinds ofinformation about your web page.

### Escape Characters
There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.)
Therefore, if you want these characters to appear on your page you need to use what aretermed "escape" characters (also known as escape codes or
entity references).

+ " is replaced with  & quot;
+ & is replaced with  & amp;
+ < is replaced with  & lt;
+ -> is replaced with  & gt;

To see more escape characters vist [HTML Entity](https://www.freeformatter.com/html-entities.html)

## HTML Layout
#### < header> < footer>

The < header> and < footer> elements can be used for:
+ The main header or footer that appears at the top or bottom of every page on the site.
+ A header or footer for an individual < article> or < section> within the page.

#### < nav>

The < nav> element is used to contain the major navigational blocks on the site such as the primary site navigation.

#### < article>

The < article> element acts as a container for any section of a page that could stand alone and potentially be syndicated.

#### < aside>

The < aside> element has two purposes, depending on whether it is inside an < article> element or not.

#### < section>

The < section> element groups related content together, and typically each section would have its own heading.

#### Heading Groups
< hgroup>

The purpose of the < hgroup> element is to group together a set of one or more < h1> through< h6> elements so that they are treated as one single heading.

#### Figures
< figure> < figcaption>

It can be used to contain any content that is referenced from the main flow of an article (not just images).

Examples of usage include:
* Images
* Videos
* Graphs
* Diagrams
* Code samples
* Text that supports the main body of an article


#### Linking Around Block-Level Elements

< a> element around a block level element that contains child elements. This allows you to turn an entire block into a link.

## Helping Older Browsers Understand
Older browsers that do not know the new HTML5 elements will automatically treat them as inline elements. Therefore, to help older browsers, you should include the line of CSS on the left which states which new elements should be rendered as block-level elements.

To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.

## Design HTML Page 
### Who is the Site For?
Every website should be designed for the target audience—not just for yourself or the site owner. It is therefore very important to understand who your target audience is.

#### Target Audience: individuals
* What is the age range of your target audience?
* Will your site appeal to more women or men? What is the mix?
* Which country do your visitors live in?
* Do they live in urban or rural areas?
* What is the average income of visitors?
* What level of education do they have?
* What is their marital or family status?
* What is their occupation?
* How many hours do they work per week?
* How often do they use the web?
* What kind of device do they use to access the web?

#### Target Audience: Companies
* What is the size of the company or relevant department?
* What is the position of people in the company who visit your site?
* Will visitors be using the site for themselves or for someone else?
* How large is the budget they control?

### Why People Visit YOUR Website
Now that you know who your visitors are, you need to consider why they are coming. While some people will simply chance across your website, most will visit for a specific reason.

### What Your Visitors are Trying to Achieve
It is unlikely that you will be able to list every reason why someone visits your site but you are looking for key tasks and motivations. This information can help guide your site designs.

### What Information Your Visitors Need
You know who is coming to your site and why they are coming, so now you need to work out what information they need in order to achieve their goals quickly and effectively.

### How Often People Will Visit Your Site
Some sites benefit from being updated more frequently than others. Some information (such as news) may be constantly changing, while other content remains relatively static.

### Site Maps
Now that you know what needs to appear on your site, you can start to organize the information into sections or pages.
The aim is to create a diagram of the pages that will be used to structure the site. This is known as a site map and it will show how those pages can be grouped.

![site map](https://nakib4tech.com/wp-content/uploads/2018/07/Sitemap_HowTo.png)

### WireFrames
A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.

![wireframe](https://d1dlalugb0z2hd.cloudfront.net/handbooks/agile-handbook/wireframe/01-youtube-wireframe-example.png)

__Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.__

__You can differentiate between pieces of information using size, color, and style.__

__You can use grouping and similarity to help simplify the information you present.__

## What is Script and How do I create one?
A script is a series of instructions that a computer can follow to achieve a goal.

To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.

Start with the big picture of what you want to achieve, and break that down into smaller steps.
1. DEFINE THE GOAL
2. DESIGN THE SCRIPT
3. CODE EACH STEP

Computers approach tasks in a different way than
humans, so your instructions must let the computer
solve the task prggrammatically.
To approach writing a script, break down your goal into
a series of tasks and then work out each step needed
to complete that task (a flowchart can help).

#### Designing a Script task by FlowChart
![jsFlowChart](https://cdn.ourcodeworld.com/public-media/gallery/gallery-574c2766d2832.png)

Often scripts will need to perform different tasks in different situations.
You can use flowcharts to work out how the tasks fit together.
The flowcharts show the paths between each step.

### OBJECTS (TH INGS)
In computer programming, each physical thing in the world can be represented as an object.
### PROPERTIES (CHARACTERISTICS)
Both of the cars share common characteristics. In fact, all cars have a make, a color, and engine size. You could even determine their current speed. Programmers call these characteristics the properties of an object.
### EVENTS
In the real world, people interact with objects. These interactions can change the values of the properties in these objects.
### METHODS
Methods represent things people need to do with objects. They can retrieve or update the values of an object's properties.

#### Each object can have its own:
* Properties
* Events
* Methods

Computers use data to create models of things in the real world.
The events, methods, and properties of an object all relate to each other:
Events can trigger methods, and methods can retrieve or update an object's properties.

#### WEB BROWSERS ARE PROGRAMS BUILT USING OBJECTS
Web browsers create similar models of the web page they are showing and of the browser window that the page is being shown in.

#### THE DOCUMENT OBJECT REPRESENTS AN HTML PAGE
Using the document object, you can access and change what content users see on the page and respond to how they interact with it.

#### HOW A BROWSER SEES A WEB PAGE

In order to understand how you can change the content of an HTML page using JavaScript, you need to know how a browser interprets the HTML code and applies styling to it.

1. RECEIVE A PAGE AS HTML CODE
2. CREATE A MODEL OF THE PAGE AND STORE IT IN MEMORY
3. USE A RENDERING ENGINE TO SHOW THE PAGE ON SCREEN

![exmple](https://i2.wp.com/blog.logrocket.com/wp-content/uploads/2018/09/browser-rending-behind-scenes.png?fit=730%2C375&ssl=1)

#### How do I write a script for a web Page ?
It is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the . j s extension.

The HTML < script> element is used in HTML pages to tell the browser to load the JavaScript file (rather like the < link> element can be used to load a CSS file).

If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web page that the browser has created.
