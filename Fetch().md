1. **Definition**
	- The `fetch()` API is build in javascript function used to request data from a server
	- It returns a promise, which means you handle the result using `.then()` or `.catch()` or `async / await`

2. **Syntax**
	```javaScript
	fetch(url, options)
	  .then(response => response.json())  // Convert response to JSON
	  .then(data => console.log(data))    // Use the data
	  .catch(error => console.error('Error:', error));
	```

3. **Example : Weather website**
	- Lets say we want to get Chennai weather data from a weather API
	```javaScript
	Fetch('https://api.example.com/weather?city=Chennai')
		.then(response => response.json())
		.then(data => {
			console.log(data.temperature);
			console.log(data.condition);
			
		})
		.catch(error => console.error(`Error fetching weather:`, error));
	```
	- If the API returns:
	```json
	{
		"temperature" : 32,
		"Condition" : "party cloudy"
	}
	```
	- We can use Javascript to show this on the webpage:
	```Javascript
	<p id="temp"></p>
	<p id="condition"></p>
	
	<script>
	fetch('https://api.example.com/weather?city=Chennai')
	  .then(res => res.json())
	  .then(data => {
	    document.getElementById('temp').textContent = data.temperature + "°C";
	    document.getElementById('condition').textContent = data.condition;
	  });
	</script>

```