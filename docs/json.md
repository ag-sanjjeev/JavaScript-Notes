## &#9873; JSON:
JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for developer to read and write, and easy for machines to parse and generate. It is often used to transmit data between a server and a client web application, or between different parts of a web application.

### &#9780; Overview:
1. [Parsing and Manipulating](#-parsing-and-manipulating)

### &#10022; Parsing and Manipulating:
JSON syntax is based on JavaScript object literals. It consists of key-value pairs. which is enclose with curly braces {} for objects, and square brackets [] for arrays.

*Syntax:*
```json
{
  "name": "Kumar",
  "age": 30,
  "city": "Chennai"
}
```

**Methods Involved and Used on JSON:**
It has built-in methods, which is provided in JavaScript to work with JSON:
- `JSON.parse()`: Parses a JSON string into a JavaScript object.
- `JSON.stringify()`: Converts a JavaScript object into a JSON string.

**Parsing:**
```javascript
let jsonString = '{"name": "Kumar", "age": 30}';
let jsonObject = JSON.parse(jsonString);
console.log(jsonObject.name); // Output: Kumar
```

**Manipulating:**
```javascript
jsonObject.age = 31;
jsonObject.city = "Chennai";
```

**Convert back into JSON:**
```javascript
let newJsonString = JSON.stringify(jsonObject);
console.log(newJsonString);
```

**Usages of JSON:**
- *Data exchange:* It is commonly used to transmit data between a server and client.
- *Data storage:* It can be used to store data locally in the browser using localStorage or sessionStorage.
- *Configuration files:* It is often used for configuration files due to its human-readable format and easy for machine to parsing.
- *API responses:* Most of APIs return data in JSON format.

---
[&#8682; To Top](#-json)

[&#10094; Previous Topic](./regular-expressions.md) &emsp; [Next Topic &#10095;](./web-apis.md)

[&#8962; Goto Home Page](../README.md)
