## &#9873; Arrays:

Arrays are generally [Non-Primitive Data Types](./data-types.md#-non-primitive-data-types).

Array in JavaScript are collections of value list, where the values are any data type. They represent list of values.

### &#9780; Overview:
1. [Array Methods](#-array-methods)
2. [Array Iteration](#-array-iteration)

### &#10022; Array Methods:
JavaScript provide a variety of methods for manipulating and working with arrays.

**Common Array Methods:**
- `push():` Adds elements to the end of an array.
- `pop():` Removes the last element from an array and returns it.
- `shift():` Removes the first element from an array and returns it.
- `unshift():` Adds elements to the beginning of an array.   
- `slice():` Creates a new array containing a portion of the original array.
- `splice():` Removes or replaces elements in an array.
- `concat():` Combines multiple arrays into a new array.
- `join():` Joins elements of an array into a string.
- `reverse():` Reverses the order of elements in an array.
- `sort():` Sorts elements in an array.
- `forEach():` Executes a function for each element in an array.
- `map():` Creates a new array by applying a function to each element of the original array.
- `filter():` Creates a new array containing elements that meet a certain condition.
- `reduce():` Applies a function to each element in an array to reduce it to a single value.
- `indexOf():` Returns the index of the first occurrence of an element in an array.
- `lastIndexOf():` Returns the index of the last occurrence of an element in an array.
- `includes():` Checks if an array contains a specified element.
- `find():` Returns the first element in an array that meets a certain condition.
- `findIndex():` Returns the index of the first element in an array that meets a certain condition.

```javascript
let fruits = ["apple", "banana", "orange"];

// Adding elements
fruits.push("grape");
fruits.unshift("mango");
console.log(fruits); // Output: (5) ['mango', 'apple', 'banana', 'orange', 'grape']

// Removing elements
let removedFruit = fruits.pop();
console.log(removedFruit); // Output: grape
console.log(fruits); // Output: (4) ['mango', 'apple', 'banana', 'orange']

// Creating a new array
let slicedFruits = fruits.slice(1, 3);
console.log(slicedFruits); // Output: (2) ['apple', 'banana']
console.log(fruits); // Output: (4) ['mango', 'apple', 'banana', 'orange']

// Joining elements
let fruitString = fruits.join(", ");
console.log(fruitString); // Output: mango, apple, banana, orange
console.log(fruits); // Output: (4) ['mango', 'apple', 'banana', 'orange']

// Sorting elements
fruits.sort();
console.log(fruits); // Output: (4) ['apple', 'banana', 'mango', 'orange']

// Iterating over elements
fruits.forEach(function(fruit) {
  console.log(fruit);
}); 
/*
apple
banana
mango
orange
*/

// Mapping elements
let fruitLengths = fruits.map(function(fruit) {
  return fruit.length;
});

console.log(fruitLengths); // Output: (4) [5, 6, 5, 6]
```

### &#10022; Array Iteration:
Array iteration involves traversing each element of an array to perform operations on them. There are several ways to iterate over arrays in JavaScript.

**Iteration of Array:**
- for loop:
```javascript
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```

- for...in loop:
```javascript
for (let index in fruits) {
  console.log(fruits[index]);
}
```

- for...of loop:
```javascript
for (let fruit of fruits) {
  console.log(fruit);
}
```
- Array methods as loop:
	- forEach()
	- map()
	- filter()
	- reduce()

	*These methods provide different ways to iterate over arrays and perform operations on their elements, depending on the specific needs.*

**Note:** When comes to loop, iterations, setTimeout and setInterval. Use [`let`](./variables.md#-let). That treats as a new [`variable`](./variables.md) on each iteration. But [`var`](./variables.md#-var) overwrites that memory place.

```javascript
/* let usage */
let fruits = ["apple", "banana", "orange"];
for(let fruit of fruits) {
	setTimeout(() => { console.log(fruit) }, 1000);
}
/*
apple
banana
orange
*/

/* var usage */
let fruits = ["apple", "banana", "orange"];
for(var fruit of fruits) {
	setTimeout(() => { console.log(fruit) }, 1000);
}
/*
orange
orange
orange
*/
```

---
[&#8682; To Top](#-arrays)

[&#10094; Previous Topic](./objects.md) &emsp; [Next Topic &#10095;](./asynchronous-javascript.md)

[&#8962; Goto Home Page](../README.md)
