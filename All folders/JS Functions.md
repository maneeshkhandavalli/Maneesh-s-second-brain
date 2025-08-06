> A block of reusable code 
> It is a block code that you can name, store and run when ever you want instead of writing the same code again and again

- It takes inputs, does somethings, and can give an output
---
### Ways to create functions

1. Function Declaration
	- A function created with the `function` keyword followed by a name.

	```JavaScript
	function greet(){
	console.log("Hello World")
	}
	greet(); //Output : Hello World
	
	```
	- Hoisted - you can call it before its written in code
	
2. Function Expression
	- A function stored inside a variable.
	
	```JavaScript
	const greet = function(){
		console.log("Hello World")
	}
	greet(); 
	```
	- not hoisted - must be declared before calling
	
3. Arrow Functions (ES6)
	- A shorter way of writing a function using `=>` introduced in ES6.
	
	```JavaScript
	const greet = () => {
		  console.log("Hello there!");
	};
	greet();
	```
	- Shorter syntax.  
	- Does not have its own `this` (important later).
	
---
### [[Parameters and Return]] 
---
### [[`this` in  JS]]
---
### [[Arrow Functions]]
---
