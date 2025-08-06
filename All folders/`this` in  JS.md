## **`this` in JavaScript**

1. **Definition**
    - `this` is a special keyword that **refers to the object that is currently executing the function**.
    - Its value changes depending on **how** and **where** the function is called — not where it’s written.
2. **Key Rules for `this`**
    1. Global Scope:
        - In browsers, `this` refers to the `window` object
        ```JavaScript  
        console.log(this); // window (in browsers)
		```
	2.  **Inside a Function (Normal Function)**
		- In **non-strict mode**, `this` inside a function refers to the **global object**.
		- In [[strict mode]], `this` is `undefined`.
		```JavaScript  
        function test() {
		  console.log(this);
		}
		test(); // window (non-strict) / undefined (strict mode)
		```
	3. **Inside an object method**
		- When a function is called as a method of an object, `this` refers to that object