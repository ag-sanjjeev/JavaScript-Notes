## &#9873; DOM Manipulation:
DOM is stands for Document Object Model. A tree-structured representation of an HTML document, providing a programmatic interface to access and manipulate elements, attributes, and content.

*DOM Manipulation is the process of dynamically modifying the structure, content, or style of an HTML document using JavaScript.*

### &#9780; Overview:
1. [Selecting elements](#-selecting-elements)
2. [Creating elements](#-creating-elements)
3. [Adding elements](#-adding-elements)
4. [Modifying elements](#-modifying-elements)
    - [Modifying attributes](#-modifying-attributes)
    - [Changing styles](#-changing-styles)
5. [Removing elements](#-removing-elements)
6. [Event Handling](#-event-handling)
    - [Attaching event listeners](#-attaching-event-listeners)
    - [Handling events](#-handling-events)

### &#10022; Selecting elements:
To select a HTML element via JavaScript for DOM manipulation.

*Syntax:*
```javascript
document.getElementById(id);
document.getElementsByTagName(tagName);
document.getElementsByClassName(className);
document.querySelector(selector);
document.querySelectorAll(selector);
```

```javascript
let elementById = document.getElementById("myElement");
let elementsByTagName = document.getElementsByTagName("p");
let elementsByClassName = document.getElementsByClassName("myClass");
let firstElementBySelector = document.querySelector("div#submit-button");
let allElementsBySelector = document.querySelectorAll("div.myClass");
```

### &#10022; Creating elements:
To create an HTML element using DOM manipulation.

*Syntax:*
```javascript
let newElement = document.createElement(tagName);
```

```javascript
let newParagraph = document.createElement("p");
```

### &#10022; Adding elements:
To add create HTML element in the DOM tree.

*Syntax:*
```javascript
parentElement.appendChild(childElement);
parentElement.insertBefore(childElement, referenceElement);
```

```javascript
let container = document.getElementById("container");
container.appendChild(newParagraph);
```

### &#10022; Modifying elements:
To modify the HTML element as changing their properties or removing.

### &#10022; Modifying attributes:
To modifying the attributes and properties of the HTML elements.

*Syntax:*
```javascript
element.setAttribute(attributeName, attributeValue);
element.getAttribute(attributeName);
```

```javascript
let link = document.createElement("a");
link.setAttribute("href", "https://arathinai.blogspot.com");
link.setAttribute("target", "_blank");
```

### &#10022; Changing styles:
To changing the default or initial style of an element.

*Syntax:*
```javascript
element.style.propertyName = propertyValue;
```

```javascript
let heading = document.querySelector("h1");
heading.style.color = "blue";
heading.style.fontSize = "24px";
```

### &#10022; Removing elements:
To remove an element from the DOM tree.

*Syntax:*
```javascript
parentElement.removeChild(childElement);
```

```javascript
container.removeChild(newParagraph);
```

### &#10022; Event Handling:
*Events:* Actions that occur in a web page, such as clicks, key presses, or mouse movements.

### &#10022; Attaching event listeners:
To listen for an event occurrence of an element, That need to be attach specific type of event.

*Syntax:*
```javascript
element.addEventListener(eventType, eventHandler);
```

```javascript
let button = document.getElementById("myButton");
button.addEventListener("click", function() {
  console.log("Button clicked!");
});
```

### &#10022; Handling events:
*Event Handling:* The process of responding to events in a web page using JavaScript.

**Common events:**
- click
- mouseover
- mouseout
- keydown
- keyup
- submit
- change
- load
- resize
- scroll

**Custom events:**
Create own events using dispatchEvent() and addEventListener().

```javascript
// Create a custom event
let myCustomEvent = new Event("myCustomEvent");

// Dispatch the event
document.dispatchEvent(myCustomEvent);

// Listen for the event
document.addEventListener("myCustomEvent", function() {
  console.log("Custom event fired!");
});
```

---
[&#8682; To Top](#-dom-manipulation)

[&#10094; Previous Topic](./functions.md) &emsp; [Next Topic &#10095;](./objects.md)

[&#8962; Goto Home Page](../README.md)
