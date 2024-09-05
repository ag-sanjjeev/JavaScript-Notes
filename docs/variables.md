## &#9873; Variables
The variables in JavaScript allows to store data to the names. That can be used again in the code.

*There are 3 common variables in JavaScript.*

### &#9780; Overview:
1. [var](#-var)
2. [let](#-let)
3. [const](#-const)
4. [comparison](#-comparison)

### &#10022; Var:
It declares a function-scoped or globally scoped variable. The scope means accessibility of the data which can be accessible inside function or if defined globally can accessible through out of the code.

*Syntax: `var variableName = value;`*

```javascript
var x = 10;
console.log(x); // Output: 10
```

### &#10022; Let:
It declares a block-scoped variable. The data can be accessible block level of the code.

*Syntax: `let variableName = value;`*

```javascript
function myFunction() {
  let y = 5;
  console.log(y); // Output: 5
}
````

### &#10022; Const:
It declares a constant variable whose value cannot be changed after it's assigned.

*Syntax: `const variableName = value;`*

```javascript
const PI = 3.14159;
console.log(PI); // Output: 3.14159
````

### &#10022; Comparison:
- Scope:
  - `var`: Function-scoped or globally scoped.
  - `let` and `const`: Block-scoped.
- Redeclaration:
  - `var`: Can be redeclared within the same scope.
  - `let` and `const`: Cannot be redeclared within the same scope.
- Reassignment:
  - `var` and `let`: Can be reassigned.
  - `const`: Cannot be reassigned.

| var | let | const |
| --- | --- | --- |
|  For older JavaScript code or when you need function-scoped or globally scoped variables. | For declaring variables within blocks (e.g., functions, loops, conditionals) where you need block-scoped behavior. | For declaring variables that will not change their values, such as constants or immutable objects. This helps prevent accidental modifications and improves code readability. |

---
[&#8682; To Top](#-variables)

[&#10094; Previous Topic](./basic-syntax.md) &emsp; [Next Topic &#10095;](./data-types.md)

[&#8962; Goto Home Page](../README.md)
