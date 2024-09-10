## &#9873; Asynchronous JavaScript:
Asynchronous programming in JavaScript allows tasks to run independent of the main thread execution without disturbing it. This performs operations independent of the main thread execution like fetching data from a server, handling user input, etc., 

*It performing time-consuming tasks without freezing the UI.*

*These operations don't block the main thread and allowing other parts of your code continuously executing while the asynchronous task is in progress.*

### &#9780; Overview:
1. [Callbacks](#-callbacks)
2. [Promises](#-promises)
3. [Async/Await](#-async-await)

### &#10022; Callbacks:
Callbacks are functions that are passed as arguments to other function calls. This callbacks are executed at a later or end of the function or typically when an asynchronous operation completes.

```javascript
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => {
    console.log(data);
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

In this above example,
- *The `fetch()` function returns a Promise,*
- *That promise is then resolved with the response data.* 
- *The `.then()` method is used to handle the resolved value.* 
- *The `.catch()` method is used to handle potential errors.*

### &#10022; Promises:
Promises are objects that represent the eventual completion or failure of an asynchronous operation. They provide a more structured and readable way to handle asynchronous code compared to callbacks.

```javascript
function fetchData() {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      resolve('Data fetched successfully');
    }, 2000);
  });
}

fetchData()
  .then(data => {
    console.log(data);
  })
  .catch(error => {
    console.error('Error:', error);
  });
``` 

In this above example,
- *Promises can either be resolved or rejected.*
- *The `.then()` method is used to handle the resolved value.*
- *While the `.catch()` method is used to handle rejection.*

### &#10022; Async Await:
Using `async` and `await` for Cleaner Asynchronous Code.
- `async`: Declares a function as asynchronous.
- `await`: Pauses the execution of an `async` function until a Promise is resolved.

```javascript
async function fetchData() {
  const data = await fetch('https://api.example.com/data');
  const json = await data.json();
  console.log(json);
}

fetchData();
```

---
[&#8682; To Top](#-asynchronous-javascript)

[&#10094; Previous Topic](./arrays.md) &emsp; [Next Topic &#10095;](./error-handling.md)

[&#8962; Goto Home Page](../README.md)
