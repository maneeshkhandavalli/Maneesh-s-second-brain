1. Definition:
	- A promise in javascript is a action that happens in the future
	- There are three states
		1. Pending -> Task hasn't finished yet.
		2. Fulfilled -> task completed successfully 
			-  .then() runs
		3. Rejected -> Task failed
			- .catch() runs

2. Why is it useful?
	- Websites often need data from a server, like a leaning management system loading courses
	- fetching that data takes time, but we dont want the website to freeze while waiting
	- promises let the rest of the site working while waiting for the data

3. Basic Syntax
	```JavaScript
	let myPromise = new Promise((resolve, reject) => {
	  let success = true;
	
	  if (success) {
	    resolve("Data loaded successfully");
	  } else {
	    reject("Error loading data");
	  }
	});
	
	myPromise
	  .then(result => console.log(result)) // if resolved
	  .catch(error => console.log(error)); // if rejected

	```
	