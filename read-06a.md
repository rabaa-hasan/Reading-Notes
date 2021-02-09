# BASIC JAVASCRIPT INSTRUCTIONS
It is a fast, interactive Programming language. Java Script excuted line by line. It has a lot of data types such as String, Number, Boolean and Variable(to save value can be changed later than).
Browsers require very detailed instructions about what we want them to do. Therefore, complex scripts can run to hundreds (even thousands) of lines. Programmers use functions, methods, and objects to organize their code.
## JavaScript Functions
A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).
* When an event occurs (when auser clicks a button)
* When it is invoked (called) from JavaScript code
* Automatically (self invoked)

You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.

* Function parameters are listed inside the parentheses () in the function definition.

* Function arguments are the values received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.

A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

The code to be executed, by the function, is placed inside curly brackets: {}.

function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
![function](https://s3.ap-south-1.amazonaws.com/s3.studytonight.com/tutorials/uploads/pictures/1587882057-1.png)
## Function declaration

function isEven(num) {
  return num % 2 === 0;
}

isEven(24); // => true

isEven(11); // => false

### function can be called by its name: showMessage().

For instance:

function showMessage()

 {

  alert( 'Hello everyone!' );

}

showMessage();

showMessage();

### Outer variables
A function can access an outer variable as well, for example:

let userName = 'John';

function showMessage() 
{

  let message = 'Hello, ' + userName;

  alert(message);
}

showMessage(); 
// Hello, John