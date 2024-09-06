## &#9873; Functions
Functions are reusable blocks of code that perform specific tasks. It helps to organize the code, make it more modular, and for code reusability.

### &#9780; Overview:
1. [Defining functions](#-defining-functions)
2. [Calling functions](#-calling-functions)
3. [Function arguments and return values](#-function-arguments-and-return-values)
4. [Function Scope and closures](#-function-scope-and-closures)
5. [Arrow functions](#-arrow-functions)

### &#10022; Defining Functions:
The functions are usable before defining it.

*Syntax:*
```javascript
function functionName(parameter1, parameter2, ...) {
  // Function body (statements to be executed)
  return value; // Optional: Returns a value
}
```

```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}
```

### &#10022; Calling Functions:
To use function in the JavaScript code, that need to be called where it is required.

*Syntax:*
```javascript
functionName(argument1, argument2, ...);
```

```javascript
greet("Kumar"); // Output: Hello, Kumar!
```

### &#10022; Function Arguments and Return Values:
**Arguments:** Values passed to a function that accepts as parameter of it when it's called.
**Return Values:** Values that a function can return to the where it was called or invoked using the return statement in the function.

```javascript
function add(a, b) {
  return a + b;
}

let sum = add(1, 2);
console.log(sum); // Output: 3
```

### &#10022; Function Scope and Closures:
**Scope:** The region of code where a variable or function is accessible.
**Closures:** Functions that have access to variables from the outer scope, even after the outer scope has finished executing.

```javascript
function outerFunction() {
  let x = 10;

  function innerFunction() {
    console.log(x); // Accesses the outer variable x
  }

  return innerFunction;
}

let closure = outerFunction();
closure(); // Output: 10
```

### &#10022; Arrow Functions:
It is defined in a concise way or in shorthand form.

*Syntax:*
```JavaScript
(parameters) => expression;
```

```javascript
let greet = (name) => {
  console.log("Hello, " + name + "!");
};
```

---
[&#8682; To Top](#-functions)

[&#10094; Previous Topic](./control-flow.md) &emsp; [Next Topic &#10095;](./dom-manipulation.md)

[&#8962; Goto Home Page](../README.md)
