# JavaScript summary
These are my notes from learning the JavaScript language. I have used several resources to learn the language, the notes are inspired from all these resources. I have used two Udemy courses, video's on YouTube, a book, online resources and two learning environments. 

Video resources:
[JavaScript: Understanding the Weird Parts](https://www.udemy.com/course/understand-javascript/)
[Advanced JavaScript Concepts](https://www.udemy.com/course/advanced-javascript-concepts/)
[Learn JavaScript - Full Course for Beginners](https://www.youtube.com/watch?v=PkZNo7MFNFg)

Text resources:
[Eloquent Javascript](https://eloquentjavascript.net/Eloquent_JavaScript.pdf)
[MDN JavaScript docs](https://developer.mozilla.org/en/docs/Web/JavaScript)

The learning environments:
[FreeCodeCamp](https://learn.freecodecamp.org/)
[CodeCademy](https://www.codecademy.com/learn/introduction-to-javascript)

Scrimba environments:
[Modern JavaScript](https://scrimba.com/playlist/p7v3gCd)


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

**Comments**
```js
// This is an in-line comment.
```
```js
/* This is a
multi-line comment */
```

**Variables**

Declare (unitialized) variables.
```js
var ourName;
let ourName;
const ourName;
```

Set variable.
```js
var ourName = 5;
```

Add or remove from variable.
```js
var myVar = 1;
myVar += 5; (or myVar -= 5;)
console.log(myVar); // Returns 6 or 4
```

**Escaping**
```js
\'	single quote
\"	double quote
\\	backslash
\n	newline
\r	carriage return
\t	tab
\b	word boundary
\f	form feed
```

Escaping with double quotes.
```js
var myStr = "I am a \"double quoted\" string inside \"double quotes\";
console.log(myStr);
```

Escaping with single quotes and backticks.
```js
var myStr = `'<a href="http://www.example.com" target="_blank">Link</a>'`;
console.log(myStr);
```


**Data types**







**Operators**





**Functions**




**Objects**






**Arrays**

array.push()
```js
var arr = [1,2,3];
arr.push(4);
// arr is now [1,2,3,4]
```

`array.pop()` is used to "pop" a value off of the end of an array.
```js
var threeArr = [1, 4, 6];
var oneDown = threeArr.pop();
console.log(oneDown); // Returns 6
console.log(threeArr); // Returns [1, 4]
```



**Callback function**
A callback function can take a function without a name, like example below:
```javascript
function displayStaffStatus() {
  availableAirplanes.forEach(function(element){})
}
```



**Modules**
Exporting variables.

```javascript
function function1(p1, p2) {
	return console.log("function 1");
}

function function1(p1, p2) {
	return console.log("function 1");
}

export {function1, function2};
```



**Named exports**
The export keyword allows us to export objects upon declaration.
```javascript
export let specialty = '';
```
The same thing counts for functions.
```javascript
export function isVegetarian(){};
```
Named exports also conveniently offer a way to change the name of variables when we export or import them. We can do this with the `as` keyword.
```javascript
export { availableAirplanes as aircrafts};
```




# Promises

```javascript
const executorFunction = (resolve,reject) => { };
const myFirstPromise = new Promise(executorFunction);
```
































<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0NjU0MTU0NTRdfQ==
-->