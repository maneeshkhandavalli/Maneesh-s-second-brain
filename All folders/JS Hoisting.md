> just fucking declare all your variables at the beginning of every scope dude
### **Hoisting*
1. Definition
	- a default behavior of moving variables and function declarations to the top of their scope before code execution
	- This means you can use Variables and functions before you actually declare them
2. How it works
	- Only declarations are hoisted and not initializations 
	- `var` variables are hoisted and initialized with `undefined` 
	- `let` and `const` are only hoisted but not initialized
	- Function declarations are fully hoisted 
	- But function expressions and arrow functions are not hoisted in the same way
3. Syntax
	```JavaScript
	console.log(a); // undefined
	var a = 10
	```
	- This is what we see basically var hoisting
	```JavaScript
	var = a;
	console.log(a);
	a = 10;
	```
	- This is what happens behind the scenes, javascript does it
4. Real Life analogy
	- Think of hoisting like a teacher reading out names (Declaration) of students in class attendance list before session starts
	- But unless a student says Present (Initialization), they're just marked as unknow (Undefined)
5. Why its important
	- Helps you understand why some code works even if written in a different order.
	- Prevents confusion and unexpected `undefined` or `ReferenceError`.
	- Encourages better coding practices by **declaring variables before using them**
6. We now discuss on how declarations behave when hoisted 
	- This divides into three main parts
	1. Hoisting with `var`
		- Gets hoisted to the top of its scope and initialized with `undefined`
		- Access before initializations 
	2. Hoisting with `let` and `char`
		- Gets hoisted to the top of its scope but doesnt get initialized and returns a `ReferenceError` 
		- initialization happens only at the point where they are declared
	3. Hoisting with `functions` 
		1. It is fully hoisted and you can call them before they are defined
		2. for function expression
			 - If defined with `var` → hoisted as `undefined` 
			 - If declared with `let` / `count` → in temporal dead zone until initialized
			``` JavaScript
			sayHi(); // Works fine
			function sayHi() {
			  console.log("Hello!");
			}	
			sayBye(); // TypeError
			var sayBye = function() {
				console.log("Goodbye!");
			}
				```


> When writing code, knowing these differences helps us to avoid unexpected `undefined` values or runtime errors 

