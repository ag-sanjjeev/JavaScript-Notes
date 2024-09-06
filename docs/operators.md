## &#9873; Operators
Operators are represented by symbols or keywords that perform specific operations on values in JavaScript. They are used to manipulate data, create expressions, and control the flow of your code.

*There are 5 common operators in JavaScript.*

### &#9780; Overview:
1. [Arithmetic](#-arithmetic)
2. [Comparison](#-comparison)
3. [Logical](#-logical)
4. [Assignment](#-assignment)
5. [Ternary](#-ternary)

### &#10022; Arithmetic:
Arithmetic operators is used to perform mathematical operations such as addition, subtraction, multiplication, division, modulo, increment, decrement.

*Syntax:*
```javascript
+ (addition)
- (subtraction)
* (multiplication)
/ (division)
% (modulo)
++ (increment)
-- (decrement)
```

```javascript
let addition = 5 + 3; // 8
let subtraction = 5 - 3; // 2
let multiplication = 5 * 3; // 15
let division = 5 / 3; // 1
let remainder = 5 % 3; // 2
++addition; // pre-increment
addition++; // post-increment
--addition; // pre-decrement
addition--; // post-decrement
```

### &#10022; Comparison:
Comparison operators is used to compare values and return a boolean result. comparison between values done such as equal to, not equal to, strictly equal to, strictly not equal to, greater than, less than, greater than or equal to, less than or equal to.

*Syntax:*
```javascript
== (equal to)
!= (not equal to)
=== (strictly equal to)
!== (strictly not equal to)
> (greater than)
< (less than)
>= (greater than or equal to)
<= (less than or equal to)
```

```javascript
let x = 10;
let y = 5;

if (x > y) {
  console.log("x is greater than y");
}
```

### &#10022; Logical:
Logical operators is used to combine boolean values such as logical AND, logical OR, logical NOT.

*Syntax:*
```javascript
&& (logical AND)
|| (logical OR)
! (logical NOT)
```

```javascript
let isSunny = true;
let isWeekend = true;

if (isSunny && isWeekend) {
  console.log("It's a party day!");
}
```

### &#10022; Assignment:
Assignment operators is used to assign values to variables such as assignment, addition assignment, subtraction assignment, multiplication assignment, division assignment, modulo assignment.

*Syntax:*
```javascript
= (assignment)
+= (addition assignment)
-= (subtraction assignment)
*= (multiplication assignment)
/= (division assignment)
%= (modulo assignment)
```

```javascript
let salary = 2500;
salary += 500; // salary with increment of 500
```

### &#10022; Ternary:
Ternary operators is used for a shorthand way to write an if-else statement.

*Syntax: `condition ? expression1 : expression2`*

```javascript
let isAdult = age >= 18 ? "Adult" : "Minor";
```

### &#10022; Comparison:
- Arithmetic Operators: 
  - For mathematical calculations, data manipulation, and creating expressions.
- Comparison Operators: 
  - For making decisions based on conditions and controlling the flow of your code.
- Logical Operators: 
  - For combining boolean values and creating complex conditions.
- Assignment Operators: 
  - For assigning values to variables and updating their values.
- Ternary Operator: 
  - For concisely writing conditional expressions.

---
[&#8682; To Top](#-operators)

[&#10094; Previous Topic](./data-types.md) &emsp; [Next Topic &#10095;](./control-flow.md)

[&#8962; Goto Home Page](../README.md)
