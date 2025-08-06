### Parameters & Return

- A **parameter** is basically a **placeholder variable** that you write in a function’s definition so the function can receive input values when it’s called.

1. **Default Parameters**
	- Lets you set a value for a parameter if no argument is passed.
	```JavaScript
	function greet(name) {  // 'name' is the parameter
	  console.log(`Hello, ${name}!`);
		}
	greet("Cosmic"); // Output: Hello, Cosmic!  ('Cosmic' is the argument)
	```

2. **Rest parameters(`...`) **
	- Packs multiple arguments into a single array
	```JavaScript
	function sum(...numbers) {
	  return numbers.reduce((total, num) => total + num, 0);
	}
	console.log(sum(1, 2, 3)); // 6
	```

3. **Spread operators(`...`)**
	- Opposite of rest it **unpacks** elements from an array or object.
	```JavaScript
	let nums = [1, 2, 3];
	let newNums = [...nums, 4, 5];
	console.log(newNums); // [1, 2, 3, 4, 5]
	```
