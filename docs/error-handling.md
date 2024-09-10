## &#9873; Error Handling:
This is a crucial aspect of JavaScript programming that involves anticipating and managing potential errors or exceptions that may occur during execution of the code. It helps to prevent unexpected crashes and stop execution flow of code. It provides a more robust and user-friendly experience in the application.

### &#9780; Overview:
1. [try and catch](#-try-and-catch)
2. [Custom error objects](#-custom-error-objects)
3. [Necessity of Error Handling](#-necessity-of-error-handling)

### &#10022; try and catch:
It is common error handling mechanism in JavaScript.

- *try:* It executes the code that may cause error.
- *catch:* It executes the code that only error in the `try` block.

*Syntax:*
```javascript
try {
  // Code that might throw an error
} catch (error) {
  // Code to be executed if an error occurs
  console.error(error);
}
```

```javascript
function divide(a, b) {
  if (b === 0) {
    throw new Error("Division by zero");
  }
  return a / b;
}

try {
  let result = divide(10, 0);
  console.log(result);
} catch (error) {
  console.error(error.message);
}
```

### &#10022; Custom error objects:
This allows to create specific error types with custom messages and properties.

*Syntax:*
```javascript
function CustomError(message) {
  this.message = message;
  this.name = "Custom Error";
}
```

```javascript
function validateAge(age) {
  if (price < 10) {
    throw new Error("Under Price");
  }
  if (age > 120) {
    throw new CustomError("Over Price");
  }
}
```

### &#10022; Necessity of Error Handling
- *Prevent unexpected crashes:* It helps to avoid unexpected application failures and provides a more stable execution and experience.
- *Provide informative error messages:* Custom error objects can provide informative and helpful error messages to users.
- *Improve code reliability:* By anticipating potential errors and handling them, It makes code more robust, less prone to bugs and execution failure.
- *Enable better debugging:* Error handling can helps to identify issue more efficiently.
- *Enhance user experience:* Informative error messages can guide users to correct errors or prevent potential data loss.

---
[&#8682; To Top](#-error-handling)

[&#10094; Previous Topic](./asynchronous-javascript.md) &emsp; [Next Topic &#10095;](./regular-expressions.md)

[&#8962; Goto Home Page](../README.md)
