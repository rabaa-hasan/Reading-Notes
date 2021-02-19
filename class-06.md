# JS Object Literals; The DOM
## Understanding The Problem Domain Is The Hardest Part Of Programming
What is the hardest thing about writing code?

* Learning a new technology
* Naming things
* Testing your code
* Debugging
* Fixing bugs
* Making software maintainable

The real world is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.
Programming is easy if you understand the problem domain

If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

1. Make the problem domain easier
2. Get better at understanding the problem domain

You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.

## WHAT IS AN OBJECT?
Objects group together a set of __variables__ and __functions__ to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

#### IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES
#### IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS

![object](Screenshot(8).png)

## THE DOM TREE IS A MODEL OF A WEB PAGE
As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.

![dom](https://miro.medium.com/max/1200/1*5zKczvG219FSLibHQH4jSA.png)

### WORKING WITH THE DOM TREE
Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.

### caching dom query

![domQ](Screenshot(10).png)

You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.

Whenever a DOM query can return more than one node, it will always return a Nade list.

From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.

An element node can contain multiple text nodes and child elements that are siblings of each other.

Browsers offer tools for viewing the DOM tree .

[DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)
