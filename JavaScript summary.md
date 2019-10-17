# JavaScript summary
These are my notes from learning the JavaScript language. I have used several resources to learn the language, the notes are inspired from all these resources. I have used two Udemy courses, a book, online resources and two learning environments. 

The Udemy courses:
[JavaScript: Understanding the Weird Parts](https://www.udemy.com/course/understand-javascript/)
[Advanced JavaScript Concepts](https://www.udemy.com/course/advanced-javascript-concepts/)

Text resources:
[Eloquent Javascript](https://eloquentjavascript.net/Eloquent_JavaScript.pdf)
[MDN JavaScript docs](https://developer.mozilla.org/en/docs/Web/JavaScript)

The learning environments:
[FreeCodeCamp](https://learn.freecodecamp.org/)
[CodeCademy](https://www.codecademy.com/learn/introduction-to-javascript)



## Language characteristics

**Syntax parsers**
A program that reads your code and determines what it does and if it's grammar is valid.

**Single threaded**
One set of instructions is executed every single time. It has only one call stack. Web API requests are asynchronous.

**Deterministic**
Whatever we put into the parameters it always returns the same values.



## Scope

**Scope chain**
Scope chain [example](https://repl.it/@aneagoie/Scope-Chain). Scope leakage [example](https://repl.it/@aneagoie/JS-is-Weird).



**Function scope vs block scope**
Block scoping means declaring a variable not just inside a function, but around any curly brackets.




## Lexical

**Hoisting**
The behavior of moving the variables (only var) and functions to the top of their respective environment (during compilation). Use let or const keyword to prevent hoisting. Hoisting [example](https://repl.it/@aneagoie/hoisting-exe).


**Lexical environment**
Where you write something. Used so compiler can understand where to put things/what actions to undertake.


**Lexical scope**
In JavaScript our lexical scope (available data + variables where the function was defined) determines our available variables. Not where the function is called (dynamic scope).


**IIFE pattern**
Explained in this Udemy lesson.


**Execution context**
Execution context tells you which lexical environment is running. There are lots of lexical environments. Which one is currently running is managed via execution contexts. It can contain things beyond what you've written in your code. Each execution context has it's own variable environment.


**Variable environment**
Each execution context has it's own variable environment. [Example](https://repl.it/@aneagoie/Variable-Environment).

Types of execution context:
 - Global
 - Local
 
Global execution context:
 - this
 - arguments
 - window


## Syntax


**Variables**




**Operators**





**Functions**









**Modules**
Exporting modules.

```javascript
function function1(p1, p2) {
	return console.log("function 1");
}

function function1(p1, p2) {
	return console.log("function 1");
}

export { function1, function2};
```
