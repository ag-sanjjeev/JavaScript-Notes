## &#9873; Introduction
This introduction will give explanation about creating and using JavaScript in the HTML.

### &#10022; What is Vanilla JavaScript?
Vanilla JavaScript is the pure, original version of JavaScript, without any additional frameworks or libraries. It's the basic and foundation for many modern web technologies are built.

### &#10022; What is the need for it?
* **Understanding the Basics:** Learning Vanilla JavaScript will provides a strong foundation for understanding about How web pages are work? and How it interact with users?.
* **Flexibility:** Vanilla JavaScript offers maximum control and flexibility for building the custom solutions tailored to meet specific needs.
* **Compatibility:** It's compatible with all modern web browsers, ensuring that script works across different devices and platforms.

### &#10022; Getting Started:
1. **Text Editor:** Choose a text editor or professional code editors..
2. **HTML File:** Create a new HTML file (e.g., `index.html`) and open it in your text editor.
3. **Basic Structure:** Add the basic HTML structure:

 ```html
 <!DOCTYPE html>
 <html>
 <head>
     <title>My First JavaScript Page</title>
 </head>
 <body>
     <h1 id="heading"></h1>
     <script src="script.js"></script>
 </body>
 </html>
 ```

4. **Create JavaScript File:** Create a new JavaScript file (e.g., `script.js`) and link it to your HTML file using the [`<script>`](https://github.com/ag-sanjjeev/HTML-Notes/blob/master/tags/script-tag.md) tag.

**Example:**
```javascript
// Variables
let message = "Hello, World!";

// DOM Manipulation
let heading = document.getElementById("heading");
heading.textContent = message;
```

5. **Running JavaScript:** 
	- Then **`select the html file`** and run by hitting the **`ENTER`** button 
	- Or by **`open`** or by **`open with`** option menu associated with that selected file.
	- After that above actions will be reflected on the web browser.

6. **Best Practices:**
	- Instead of js files, You can directly write JavaScript for the HTML document via [Script Tag](https://github.com/ag-sanjjeev/HTML-Notes/blob/master/tags/script-tag.md).
	- The best practice is, Write separate file for JavaScript file to make HTML document clean and neat in the code. And also it gives the code re-usability. 

---
[&#8682; To Top](#-introduction)

[&#10094; Previous Topic](./README.md)&emsp;[Next Topic &#10095;](./topics.md)

[&#8962; Goto Home Page](./README.md)