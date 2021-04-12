# The JavaScript Call Stack
## Call Stack

Call stack is a data structure that uses ther last in, first out (LFO) principle to temporarily store and manage function invocation.

__LIFO__: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

Handling function calls. When the code is run:

* When secondFunction() gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.
* secondFunction() then calls firstFunction()which is pushed into the stack.
* firstFunction() returns and prints “Hello from firstFunction” to the console.
* firstFunction() is pop off the stack.
* The execution order then move to secondFunction().
* secondFunction() returns and print “The end from secondFunction” to the console.
* secondFunction() is pop off the stack, clearing the memory.

## Javascript Errors
* Reference Errors
* Range Errors
* Type Errors
* Debugging
* Call Stack
* Handling Errors

