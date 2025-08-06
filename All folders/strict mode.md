1. **Definition**
	- Strict mode is a special mode in JavaScript that **makes the language more strict and safe** by catching common coding mistakes and throwing more errors.
	- You turn it on by writing `"use strict"` at the top of a file or at the start of a function
		```JavaScript
		"use strict"
		```
2. **Main Differences Between Strict & Non-Strict Mode**

| Feature                             | Non-Strict Mode (Default)           | Strict Mode (`"use strict"`) |
| ----------------------------------- | ----------------------------------- | ---------------------------- |
| **Using undeclared variables**      | Allowed (creates a global variable) | Error                        |
| **Duplicate function parameters**   | Allowed                             | Error                        |
| **`this` in a regular function**    | Refers to `window` (in browsers)    | `undefined`                  |
| **Assigning to read-only property** | Fails silently                      | Error                        |
| **Deleting undeletable properties** | Fails silently                      | Error                        |
3. **Why use strict mode?**
	- Catches **silent errors** so you know when you mess up.
	- Prevents bad coding practices.
	- Makes your code safer and cleaner.

---