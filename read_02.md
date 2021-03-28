# jQuery, Events, The  DOM and Pair Programming
## jQuery

![jq](https://monirulalom.com/article/i-don-t-hate-jquery/jquery-logo-blue.png)

jQuery offers a simple way to achieve a variety of common JavaScript tasks quickly and consistently, across all major browsers and without any fallback code needed.

#### jQuery is a JavaScript Library.

### WHY USE JQUERY?
1. SIMPLE SELECTORS
2. COMMON TASKS IN LESS CODE
3. CROSS-BROWSER COMPATIBILITY

### jQuery Selectors
jQuery selectors allow you to select and manipulate HTML element(s).

jQuery selectors are used to "find" (or select) HTML elements based on their name, id, classes, types, attributes, values of attributes and much more. It's based on the existing CSS Selectors, and in addition, it has some own custom selectors.

All selectors in jQuery start with the dollar sign and parentheses: $().

### jQuery Event Methods
What are Events?
All the different visitors' actions that a web page can respond to are called events.

An event represents the precise moment when something happens.

Examples:

* moving a mouse over an element
* selecting a radio button
* clicking on an element
* The term "fires/fired" is often used with events. 

Example: "The keypress event is fired, the moment you press a key".

|Mouse Events|	Keyboard Events|	Form Events	|Document/Window Events|
|:--------------|:---------------------|:---------------|:---------------------|
|click	|keypress	|submit	|load|
|dblclick	|keydown|	change|	resize|
|mouseenter|	keyup|	focus|	scroll|

### jQuery Syntax For Event Methods
`$("p").click();`

You must pass a function to the event:
```
$("p").click(function(){
  // action goes here!!
});
```

### LOOPING
With jQuery, when a selector returns multiple elements, you can update all of them using the one method. There is no need to use a loop.

```
$('l i em') .addClass('seasonal ') ;
$( ' li .hot') .addClass('favorite');
```

### CHAINING
If you want to use more than one jQuery method on the same selection of elements, you can list several methods at a time using dot notation to separate.

```
$( 'l i [i d!="one"] ') . hide() .delay(SOO) . fadeln(1400);
```

## Pair Programming
### How does pair programming work?
While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

### Why pair program?
Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness