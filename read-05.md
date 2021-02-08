# Functions, Methods and Objects in Java Script
Functions allow you to group a set of related
statements together that represent a single task. Functions can take parameters (informatiorJ required
to do their job) and may return a value.

example:

offerPrice : function() {
var offerRate = this.roomRate * ((100 - this.discount) I 100);
return offerRate;

An object is a series of variables and functions that
represent something from the world around you.variables are known as properties of the
object; functions are known as methods of the object. Web browsers implement objects that represent both
the browser window and the document loaded into the
browser window.

JavaScript also has several built-in objects such as __String, Number, Math, and Date.__
## Evaluating Conditions & Conditional Statements
### Evaluating Conditions
As logical expressions are evaluated left to right, they are tested for possible "short-circuit" evaluation using the following rules:

* false && anything is short-circuit evaluated to false.
* true || anything is short-circuit evaluated to true.

### Conditional Statements
Very often when you write code, you want to perform different actions for different decisions.

You can use conditional statements in your code to do this.

In JavaScript we have the following conditional statements:

Use if to specify a block of code to be executed, if a specified condition is true

Use else to specify a block of code to be executed, if the same condition is false

Use else if to specify a new condition to test, if the first condition is false
## USING IF ... ELSE STATEMENTS
 allows you to provide two sets of code:
1. one set if the condition evaluates to true
2. another set if the condition is false

There is no need to provide an else
option. (You can just use an if
statement.)
## switch statement 
A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value.
example:

switch (level)

{

case 'One ':

title= 'Level 1 ' ;

break;

case 'Two':

tit 1 e = ' Level 2 ' ;

break;

default :

title= 'Test';

break;

}
## Comparison Operators
==	equal to

===	equal value and equal type

!=	not equal

!==	not equal value or not equal typ

(>)	greater than

(<)	less than

(<=)	less than or equal to

(>=)	greater than or equal to



## DATA TYPE PURPOSE
string    Text

number Number

Boolean true or false

nul 1 Empty value

undefined Variable has been declared but not yet assigned a value