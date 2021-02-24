# Error Handling & Debugging
### ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run:
```
2. function greetUser () {
     return 'Hello ' + getName ();
    }

3.function getName() {
    var name= 'Molly ' ;
    return name;
  }

1. var greeting= greetUser();
4. alert(greeting);
```
### EXECUTION CONTEXTS
The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.

![execution](https://ui.dev/post-images/global-variables-in-execution-phase.png)

### The stack
Stacks are data structures that follow the Last-In-First-Out (LIFO) principle, meaning the last item inserted into a stack is the first one to be deleted .
```
let a = 'Hello World!';
function first() {
  console.log('Inside first function');
  second();
  console.log('Again inside first function');
}
function second() {
  console.log('Inside second function');
}
first();
console.log('Inside Global Execution Context');
```


An Execution Context Stack for the above code.
![stack](https://miro.medium.com/max/1000/1*ACtBy8CIepVTOSYcVwZ34Q.png)

### EXECUTION CONTEXT & HOISTING
Each time a script enters a new execution context, there are two phases of activity:
1. PREPARE
 * The new scope is created
 *   Variables, functions, and arguments are created
  * The value of the this keyword is determined

2. EXECUTE
* Now it can assign values to variables
* Reference functions and run their code
* Execute statements 

#### Execution Context
![context](https://miro.medium.com/max/700/1*e-A-jDYmBTIfN2ADj13iaw.png)


#### HOISTING
![HOISTING](https://devopedia.org/images/article/287/2146.1601975565.png)

### UNDERSTANDING SCOPE
In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.

#### Global scope
![Global scope](https://ringojs.org/documentation/images/scriptscope.png)

### UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code.

### Error Objects
Error objects can help you find where your mistakes are and browsers have tools to help you read them.

There are seven types of built-in error objects in JavaScript.

```
Error : Generic error - the other errors are all based upon this error

Syntax Error: Syntax has not been followed

Ref erenceError: Tried to reference a variable that is not declared/within scope

TypeError: An unexpected data type that cannot be coerced

Range Error: Numbers not in acceptable range

URI Error: encodeURI ().decodeURI(),and similar methods used incorrectly

Eval Error: eva l () function used incorrectly.
```

![error](https://images.ctfassets.net/cj4mgtttlyx7/4EEmNj7G9MdsYn1FrKaYyh/cfe042f855745406ec03691ee942ad53/cannot-set-property.png)

### HOW TO DEAL WITH ERRORS
There are two things you can do with the errors:
1. DEBUG THE SCRIPT TO FIX ERRORS
2. HANDLE ERRORS GRACEFULLY

### A DEBUGGING WORKFLOW
Debugging is about deduction: eliminating potential causes of an error.

* WHERE IS THE PROBLEM?
* WHAT EXACTLY IS THE PROBLEM?

The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.

![error](https://infoheap.com/wp-content/uploads/2016/03/chrome-developer-tools-console-javascript-errors.png)

If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. 
