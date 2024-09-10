## &#9873; Regular Expressions:
A regular expression, often abbreviated as `regex`. It is a sequence of characters that defines a search pattern. It's used to match, find, replace, or manipulate text based on given patterns.

### &#9780; Overview:
1. [Creating regular expressions](#-creating-regular-expressions)
2. [Common regular expression patterns](#-common-regular-expression-patterns)
3. [Matching patterns in strings](#-matching-patterns-in-strings)

### &#10022; Creating regular expressions:
Regular expressions can be created in two ways:
- Literal notation:
  ```javascript
  let pattern = /pattern/;
  ```
- Constructor:
  ```javascript
  let pattern = new RegExp("pattern");
  ```

**Flags:**
Regular expressions can have flags that modify their behavior:
- `i`: Case-insensitive matching.
- `g`: Global matching, finding all matches instead of just the first.
- `m`: Multiline matching, allowing `^` and `$` to match the beginning and end of lines, respectively.

### &#10022; Common regular expression patterns:
- `.`: Matches any character except a newline.
- `^`: Matches the beginning of a string or line.
- `$`: Matches the end of a string or line.
- `*`: Matches zero or more occurrences of the preceding character or group.
- `+`: Matches one or more occurrences of the preceding character or group.
- `?`: Matches zero or one occurrence of the preceding character or group.   
- `{n}`: Matches exactly n occurrences of the preceding character or group.
- `{n,}`: Matches at least n occurrences of the preceding character or group.   
- `{n,m}`: Matches between n and m occurrences of the preceding character or group.   
- `|`: Matches either the expression before or after it.
- `()`: Groups a part of the regular expression.
- `[ ]`: Matches any character within the brackets.
- `[^ ]`: Matches any character not within the brackets

### &#10022; Matching patterns in strings:
```javascript
let text = "The quick brown fox jumps over the lazy dog.";
let pattern = /fox/;

let match = text.match(pattern);
console.log(match); // Output: ["fox"]

let index = text.search(pattern);
console.log(index); // Output: 16

let replacedText = text.replace(pattern, "cat");
console.log(replacedText); // Output: "The quick brown cat jumps over the lazy dog."
```

**Other Methods:**
There are several methods to work with regular expressions:

- `match()`: Finds all matches of a regular expression in a string and returns an array.
- `search()`: Finds the index of the first match of a regular expression in a string.
- `replace()`: Replaces all matches of a regular expression in a string with a new string.
- `test()`: Checks if a string matches a regular expression and returns a boolean.
- `split()`: Splits a string into an array using a regular expression as a separator.

---
[&#8682; To Top](#-regular-expressions)

[&#10094; Previous Topic](./error-handling.md) &emsp; [Next Topic &#10095;](./json.md)

[&#8962; Goto Home Page](../README.md)
