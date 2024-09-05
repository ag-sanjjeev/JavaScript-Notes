## &#9873; Data Types
Data Types is used to mention that the variable holds specific type data to handle and process without an issue.

*There are 3 common variables in JavaScript.*

### &#9780; Overview:
1. [Primitive Data Types](#primitive-data-types) 
    - [numbers](#-numbers)
    - [strings](#-strings)
    - [booleans](#-booleans)
    - [null](#-null)
    - [undefined](#-undefined) 
    - [symbols](#-symbols)
2. [Non-Primitive Data Types](#-non-primitive-data-types)
    - [Arrays](#-arrays)
    - [Objects](#-objects)

### &#10022; Primitive Data Types:
Primitive data types are the most basic building blocks of JavaScript. They represent individual piece of values, not objects.

The list of primitive data types are numbers, strings, booleans, null, undefined, symbols.

### &#10022; Numbers:
It represents numerical values, including integers and floating-point numbers.

```javascript
let age = 42; // Number Integer
let pi = 3.14; // Decimals Floating-point number
```

### &#10022; Strings:
It represents sequences of characters.

```javascript
let name = "Alice";
let message = "Welcome!";
````

### &#10022; Booleans:
It represents true or false values.

```javascript
let isAdult = true;
let isRaining = false;
````

### &#10022; Null:
It represents the absence of a value.

```javascript
let user = null; // Indicates that the user is not logged in
````

### &#10022; Undefined:
It represents a variable that has not been assigned a value.

```javascript
let result;
console.log(result); // Output: undefined
````

### &#10022; Symbols:
It represents a unique identifier.

*Syntax: `let uniqueSymbol = Symbol("mySymbol");`*

```javascript
const PRIVATE_KEY = Symbol("private");
````

### &#10022; Non-Primitive Data Types:
Non-primitive data types in JavaScript are complex data structures that can hold multiple values or properties. They are mutable and compared by reference.

The list of non-primitive data types are arrays and objects.

### &#10022; Arrays:
It is a ordered collections of elements.

*Syntax: `let array = [1, "hello", true];`*

```javascript
let fruits = ["apple", "banana", "orange"];
let numbers = [1, 2, 3, 4, 5];
````

See More on this [Reference](./arrays.md)

### &#10022; Objects:
It is a collections of key-value pairs

```javascript 
let object = {
  name: "Alice",
  age: 30,
  isStudent: true
};
```

See More on this [Reference](./objects.md)

### &#10022; Comparison:
- Data type:
  - Primitive Data Types: It represent individual values and single piece of data. 
  - Non-Primitive Data Types: It represent collections of data.
- Mutability:
  - Primitive Data Types: immutable (their values cannot be changed directly).
  - Non-Primitive Data Types: objects are mutable (their properties can be modified).
- Comparison:
  - Primitive Data Types: It compared by value.
  - Non-Primitive Data Types: It compared by reference.


---
[&#8682; To Top](#-data-types)

[&#10094; Previous Topic](./variables.md) &emsp; [Next Topic &#10095;](./operators.md)

[&#8962; Goto Home Page](../README.md)
