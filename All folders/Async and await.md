1. **Definition**
	- `asyn` and `await` are two keywords that make working with [[Promise in JS]] easier and look like normal step by step code.
2. **Syntax**
	```JavaScript
		async function getCourses() {
	  try {
	    let response = await fetch("https://api.example.com/courses");
	    let data = await response.json();
	    console.log(data);
	  } catch (error) {
	    console.log("Failed to load courses", error);
	  }
	}
	
	getCourses();

	```

3. **Why useful?**
	- Cleaner and easier to read than multiple .then() calls
	- Lets you write async code like its synchronous
		- one step after another
