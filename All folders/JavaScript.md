### **Basic Concepts of JS**

#### 1. **Variables**

- `var variableName = value;`
- `let variableName = value;`
- `const variableName = value;`

#### 2. **Data Types**

- String: `let str = "text";`
- Number: `let num = 123;`
- Boolean: `let flag = true;`
- Null: `let data = null;`
- Undefined: `let data;`
- Symbol: `let sym = Symbol("id");`
- BigInt: `let big = 12345678901234567890n;`
- Object: `let obj = { key: value };`
- Array: `let arr = [1, 2, 3];`
- Function: `function name(params) {}`

#### 3. **Operators**

- Arithmetic: `+`, `-`, `*`, `/`, `%`
- Assignment: `=`, `+=`, `-=`
- Comparison: `==`, `===`, `!=`, `!==`, `>`, `<`
- Logical: `&&`, `||`, `!`

#### 4. **Conditional Statements**

- `if (condition) { }`
- `else if (condition) { }`
- `else { }`
- `switch (value) { case x: break; default: }`

#### 5. **Loops**

- `for (let i = 0; i < limit; i++) { }`
- `while (condition) { }`
- `do { } while (condition);`
- `for...of`, `for...in`

#### 6. **Functions**

- Declaration: `function name(params) { }`
- Expression: `const fn = function(params) { }`
- Arrow Function: `const fn = (params) => { }`

#### 7. **Arrays and Objects**

- Access: `array[index]`, `object.key`
- Modify: `array.push()`, `object.key = value;`
- Loop: `for (let item of array)`, `for (let key in object)`
    

#### 8. **DOM Manipulation (Intro)**

- Select: `document.getElementById("id")`, `querySelector(".class")`
- Modify: `.textContent`, `.innerHTML`, `.style.property`
- Events: `element.addEventListener("click", function)`

---


### All intermediate topics

1. [[JS Scopes]]
2. [[JS Hoisting]]
3. [[JS Functions]]
4. [[JS Destructuring]] -> some pending
5. [[Ternary Operators in JS]]
6. [[Promise in JS]]
7. 