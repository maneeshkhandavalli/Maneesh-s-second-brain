Scopes in Javascipt refers to the current context of execution, which determines the accessibility of variable
	- Basically tells where variables can be used or accessed
	- for example the things inside your house (variables) you can see those but what about things inside your neighbors house? you cant see those unless your neighbors allowed to 

#### Types of Scope:

1. **Global Scope**
	- Variables declared outside any function or block are in the global scope
		```JavaScript
		let name = "Cosmic";

		function greet() {
		  console.log(name); // Accessing global variable
		}
		
	```
		### Use Case
		- Used in things like app wide settings because they can be accidently modified from anywhere
		### Real life example
		- Think of a **global variable** like a _Wi-Fi password_ set on the router. Everyone in the house can use it, but if someone changes it, it affects everyone.
2. **Function Scope**
	- Variables declared inside of a function can only be used outside of it
		```Java Scipt
		function sayHello() {
			let message = "Hello Cosmic!";
			console.log(message);
		}
		console.log(message); // ❌ Error: message is not defined
		```
		### **Use case**
		 - A function scope is helpful to encapsulate data to avoid name conflicts
		### **Real life example**
		- A function-scoped variable is like your exam hall ticket. It’s only useful in the exam hall and nowhere else.
3. **Block scope** 
	- Declared inside Curley brackets {} using  ``let`` or ``const`` 
	- only works within that block
	- useful for loops and if statements etc
		```Java Script
		if (true) {
		  const feeling = "focused";
		  console.log(feeling); // ✅ works here
		}
		console.log(feeling); // ❌ error
		```
### Table to recap everything

| Scope Type     | Declared Using        | Where It's Accessible     |
| -------------- | --------------------- | ------------------------- |
| Global Scope   | `var`, `let`, `const` | Everywhere in the script  |
| Function Scope | `var`, `let`, `const` | Inside that function only |
| Block Scope    | `let`, `const`        | Inside that `{}` block    |
