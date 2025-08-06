### Arrow Functions

1. **Definition**
    
    - An Arrow function is a shorter way to write functions in JS, introduced in ES6
    - it uses the `=>` syntax and does not have its own `this` keyword
2. **Why use it**
    
    - Shorter and cleaner code
    - Great for small, simple functions.
    - `this` inside an arrow function refers to the surrounding scope (important in React).
3. **Basic Syntax**
    
    ```javascript
    // Regular function
    function add(a, b) {
      return a + b;
    }
    // Arrow function
    const add = (a, b) => {
      return a + b;
    };
    ```

4. **`this` in arrow functions** 
	- Arrow functions **do not create their own `this`**. They use `this` from where they are created.  
	- This makes them useful for callbacks in objects or classes.
		```javascript
		   const person = {
		  name: "Cosmic",
		  normalFunc: function() {
		    console.log(this.name); // Cosmic
		  },
		  arrowFunc: () => {
		    console.log(this.name); // undefined (because 'this' is from global scope here)
		  }
		};
		
		person.normalFunc();
		person.arrowFunc();
	    ```
