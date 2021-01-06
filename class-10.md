# Code 201, 7th Jan, Read-10

## Error Handling & Debugging

First of all you need to find the source of the bug, then you need to understand the process of this piece of code so you can spot the error.

### There is two type of Errors, syntax and semantic error or logic error

Syntax **errors**, which are typographical mistakes or improper use of special characters, are **handled** by rigorous proofreading. Logic **errors**, also called bugs, occur when executed code does not produce the expected or desired result. Logic **errors** are best **handled** by meticulous program debugging.

![errors](https://infoheap.com/wp-content/uploads/2016/03/chrome-developer-tools-console-javascript-errors.png)

The JavaScript interpreter uses the concept of execution contexts. There is one global execution context;
EXECUTION CONTEXT:
* Global Context
	* Code that is in the script, but not in a function. There is only one global context in any page
* Function Context
	* Code that is being run within a function. Each function has its own function context.

* Eval Context
	
    * Text is executed like code in an internal function called eval

## Important

The most important thing is to understand variable scope, and also use the developer tools like the console in the browser and other tools to help you refractor you code and reading the errors messages so you can know where the errors happen

## Analysis During Development 

Another important thing is during system development to verify the code is working correctly even if a crash doesn't occur, or to narrow down the situations where a crash occurs. The Microsoft Access/VB6 debugger lets you step through each line of code as it runs, examine the environment (including all variables), and even change variable values and lines of code! By seeing how your code runs (which procedures get called, which IF statement branch is taken, how loops work, etc.) you gain a much better understanding of how your code work and whether it's behaving as designed.
