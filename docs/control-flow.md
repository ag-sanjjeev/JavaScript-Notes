## &#9873; Control Flow
Control flow refers to the order of the statements execution in a JavaScript program. It allows to make decisions, repeat actions, and control the flow of your code based on certain conditions.

*There are 2 Type Control Flow in JavaScript.*

### &#9780; Overview:
1. [Condition Statements](#-conditional-statements)
    - [if statement](#-if-statement)
    - [if else statement](#-if-else-statement)
    - [else if statement](#-else-if-statement)
    - [switch statement](#-switch-statement)
2. [Loops](#-loops)
    - [for loop](#-for-loop)
    - [for in loop](#-for-in-loop)
    - [for of loop](#-for-of-loop)
    - [while loop](#-while-loop)
    - [do while loop](#-do-while-loop)
- [Comparison](#-comparison)

### &#10022; Conditional Statements:
It is used to execute different code blocks based on specific conditions. There are 4 type of conditional statements. 

### &#10022; If Statement:
It executes a block of code only if a condition is true.

*Syntax:*
```javascript
if (condition) {
  // Code to be executed if condition is true
}
```

```javascript
let age = 25;

if (age >= 18) {
  console.log("You are an adult.");
}
```

### &#10022; If Else Statement:
It executes a block of code if the condition is true, otherwise it will execute an another block of code.

*Syntax:*
```javascript
if (condition1) {
  // Code to be executed if condition is true
} else {
  // Code to be executed if condition is false
}
```

```javascript
let age = 25;

if (age >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a minor");
}
```

### &#10022; Else If Statement:
It executes a block of code if the condition is true otherwise it executes another block of code when another condition is true. It also called as nested if statements.

*Syntax:*
```javascript
if (condition1) {
  // Code to be executed if condition1 is true
} else if (condition2) {
  // Code to be executed if condition1 is false and condition2 is true
}
```

```javascript
let score = 85;

if (score >= 90) {
  console.log("Excellent");
} else if (score >= 80) {
  console.log("Good");
} else {
  console.log("Needs improvement");
}
```

### &#10022; Switch Statement:
It executes different code blocks based on the value of an expression.

*Break statement is necessary to stop at specific case condition. Otherwise it will execute further statments as well.*

*Syntax:*
```JavaScript
switch (expression) {
  case value1:
    // Code to be executed if expression is equal to value1
    break;
  case value2:
    // Code to be executed if expression is equal to value2
    break;
  default:
    // Code to be executed if no case matches
    break;
}
```

```javascript
let day = "Sunday";

switch (day) {
  case "Saturday":
    console.log("It's weekend!");
    break;
  case "Sunday":
    console.log("It's weekend!");
    break;
  default:
    console.log("It's working day!");
}
```


### &#10022; Loops:
Loops are used to repeatedly execute a block of code until a certain condition is met.

*A Loop has 3 important states which are used to determine the number of times to execute.*
- Iteration Initialization
- Condition Check
- Increment/Decrement of Iteration

### &#10022; For Loop:
It executes a block of code a specified number of times.

*For loop has iteration initialization, condition check, increment/decrement of iteration are inline.*

*Syntax:*
```javascript
for (initialization; condition; increment/decrement) {
  // Code to be executed
}
```

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

### &#10022; For In Loop:
It iterates over the properties of an object.

*Syntax:*
```javascript
for (let property in object) {
  // Code to be executed
}
```

```javascript
let person = { name: "kumar", age: 30 };

for (let key in person) {
  console.log(key + ": " + person[key]);
}
```

### &#10022; For Of Loop:
It iterates over the values of an iterable object such as arrays, strings.

*Syntax:*
```javascript
for (let value of iterable) {
  // Code to be executed
}
```

```javascript
let fruits = ["apple", "banana", "orange"];

for (let fruit of fruits) {
  console.log(fruit);
}
```


### &#10022; While Loop:
It executes a block of code as long as a condition is true. This kind of loop is useful for the condition is decided based on the block of code in this loop.

*Syntax:*
```javascript
while (condition) {
  // Code to be executed
  // condition is decided based on the calculation or process or execution
}
```

```javascript
let number = 5;
var factorial = 1;
while (number > 0) {
  factorial *= number;
  number--;
}
console.log(factorial);
```

### &#10022; Do While Loop:  
It executes a block of code at least once, then repeats as long as a condition is true.

*Syntax:*
```javascript
do {
  // Code to be executed
} while (condition);
```

```javascript
let number = 5;
var factorial = 1;
do {
  factorial *= number;
  number--;
}while (number > 0);
console.log(factorial);
```

### &#10022; Comparison:
- Conditional Statements: 
  - These statements are used to decide the flow of code or execution.
- Loops: 
  - These loops are used to execute certain process or code or statements again and again. To reduce repeated lines of code.

---
[&#8682; To Top](#-control-flow)

[&#10094; Previous Topic](./operators.md) &emsp; [Next Topic &#10095;](./functions.md)

[&#8962; Goto Home Page](../README.md)
