## &#9873; Objects:

Objects are generally [Non-Primitive Data Types](./data-types.md#-non-primitive-data-types).

Objects in JavaScript are collections of key-value pairs, where the keys are properties and the values can be any data type. They represent real-world entities or concepts.

*Objects are commonly used to represent the data structures, encapsulate properties and methods, and model real-world entities. They are essential for building complex real-word JavaScript applications.*

### &#9780; Overview:
1. [Object properties and methods](#-object-properties-and-methods)
2. [Object creation](#-object-creation)
3. [Constructors](#-constructors)
4. [Methods](#-methods)
5. [Properties](#-properties)
6. [Inheritance](#-inheritance)
7. [Polymorphism](#-polymorphism)
8. [this keyword](#-this-keyword)
9. [Prototype inheritance](#-prototype-inheritance)

### &#10022; Object Properties and Methods:
Properties: Key-value pairs that define the characteristics of an object.
Methods: Functions defined within an object that operate on its properties.

### &#10022; Object Creation:
- **Literal notation:**
```javascript
let person = {
  name: "kumar",
  age: 30,
  greet: function() {
    console.log("Hello!");
  }
};
```

- **Constructor function:**
```javascript
function Person(name, age) {
  this.name = name;
  this.age = age;
}

let person = new Person("kumar", 30);
```

### &#10022; Constructors:
It is one type of functions used to create objects. It typically use the this keyword to initialize object properties.

### &#10022; Methods:
It is one type of functions defined within an object. It can access and modify the object properties.

### &#10022; Properties:
It is a key-value pairs that store data within an object.

### &#10022; Inheritance:
Inheritance is a mechanism in object-oriented programming that allows to inherit properties and methods from one object (parent or base object) to another object (child or derived object).

*Syntax:*
```javascript
class ChildClass extends ParentClass {
  // Constructor
  constructor() {
    super(); // Call the parent class's constructor
    // Additional properties or methods
  }
}
```

```javascript
class Employee {
  constructor(name) {
    this.name = name;
  }

  details() {
    console.log("Details of Employee");
  }
}

class Manager extends Employee {
  details() {
    console.log("Name: " + this.name);
  }
}

let manager = new Manager("Kumar");
manager.details();
```

### &#10022; Polymorphism:
Polymorphism is the ability of objects to respond to the same method call in different ways.

*Syntax: (Overriding methods)*
```javascript
class ChildClass extends ParentClass {
  // Override the parent class's method
  method() {
    // Custom implementation
  }
}
```

```javascript
class Employee {
  constructor(name) {
    this.name = name;
  }

  details() {
    console.log("Details of Employee");
  }
}

class Manager extends Employee {
  details() {
    console.log("Name: " + this.name);
  }
}

let manager = new Manager("Kumar");
manager.details();
```

### &#10022; this Keyword:
This refers to the current object within a method.

### &#10022; Prototype Inheritance:
Prototype Inheritance means that objects created using a constructor function inherit properties and methods from the constructor prototype.

**Prototype:** An object that serves as a template for other objects.

**Creating custom prototypes:**
*Syntax: (Modifying the prototype)*
```javascript
Object.prototype.myCustomMethod = function() {
  // Method implementation
};
```

*Syntax: (Creating a custom prototype object)*
```javascript
function MyObject() {}

MyObject.prototype.myProperty = "value";
MyObject.prototype.myMethod = function() {
  // Method implementation
};
```

---
[&#8682; To Top](#-objects)

[&#10094; Previous Topic](./dom-manipulation.md) &emsp; [Next Topic &#10095;](./arrays.md)

[&#8962; Goto Home Page](../README.md)
