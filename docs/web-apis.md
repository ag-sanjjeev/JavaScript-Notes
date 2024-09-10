## &#9873; Web APIs:
Web APIs are a set of built-in JavaScript objects that can provide an access to the browser's environment and allow web applications to interact with hardware, network resources, and other parts of the system through the browser.

### &#9780; Overview:
1. [Fetch API](#-fetch-api)
2. [WebSockets](#-websockets)
3. [Local Storage](#-local-storage)
4. [Session Storage](#-session-storage)
5. [Geolocation API](#-geolocation-api)
6. [Canvas API](#-canvas-api)
7. [Web Audio API](#-web-audio-api)
8. [Clipboard API](#-clipboard-api)
9. [Web camera API](#-web-camera-api)
10. [Microphone API](#-microphone-api)
11. [Handling Cookies](#-handling-cookies)
12. [Other APIs](#-other-apis)

### &#10022; Fetch API:
A modern API for making network requests for the data required in JavaScript.

*Syntax:*
```javascript
fetch(url, options)
  .then(response => response.json())
  .then(data => {
    // Handle the data
  })
  .catch(error => {
    // Handle errors
  });
```

```javascript
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => {
    console.log(data);
  });
```

### &#10022; WebSockets:
A protocol for establishing persistent, full-duplex communication channels between a client and a server.

*Syntax:*
```javascript
const socket = new WebSocket('ws://example.com:8080');
```

```javascript
const socket = new WebSocket('ws://example.com:8080');

socket.onopen = () => {
  console.log('WebSocket connection opened');
};

socket.onmessage = (event) => {
  console.log('Received message:', event.data);
};

socket.onclose = () => {
  console.log('WebSocket connection closed');
};
```

### &#10022; Local Storage:
It allows to store data locally in the browser for a specific domain.

```javascript
/* Setting local storage value for specific key  */
localStorage.setItem('key', 'value');
/* Reading local storage for the key */
let value = localStorage.getItem('key');
/* Removing local storage value on the key */
localStorage.removeItem('key');
/* Clearing local storage on the current site */
localStorage.clear();
```

### &#10022; Session Storage:
It allows to store data locally in the browser for a single session.

```javascript
/* Setting session storage */
sessionStorage.setItem('cart', JSON.stringify(cart));
/* Reading session storage */
let cart = JSON.parse(sessionStorage.getItem('cart'));
```

### &#10022; Geolocation API:
It provides access to the user's geographical location.

```javascript
navigator.geolocation.getCurrentPosition(successCallback, errorCallback);
```

```javascript
navigator.geolocation.getCurrentPosition(
  (position) => {
    console.log(position.coords.latitude, position.coords.longitude);
  },
  (error) => {
    console.error('Error:', error);
  }
);
```

### &#10022; Canvas API:
It allows to create 2d graphics on an HTML canvas element.

```javascript
let canvas = document.getElementById('myCanvas');
let context = canvas.getContext('2d');
context.fillStyle = 'red';
context.fillRect(10, 10, 100, 100);
```

See More on this [Canvas Reference](https://github.com/ag-sanjjeev/HTML-Notes/blob/master/tags/link-tag.md)

### &#10022; Web Audio API:
It provides an interface for creating, manipulating, and processing audio data.

*Syntax:*
```javascript
let audioContext = new AudioContext();
```

```javascript
audioContext.createOscillator().start();
```

### &#10022; Clipboard API:
It provides access to the user's clipboard.

```javascript
navigator.clipboard.writeText('Hello, world!');
navigator.clipboard.readText().then(text => console.log(text));
```

### &#10022; Web camera API:
It provides access to the user's webcam.

```javascript
navigator.mediaDevices.getUserMedia({ video: true })
  .then(stream => {
    let video = document.getElementById('myVideo');
    video.srcObject = stream;
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

### &#10022; Microphone API:
It provides access to the user's microphone.

```javascript
navigator.mediaDevices.getUserMedia({ audio: true })
  .then(stream => {
    let audioContext = new AudioContext();
    let source = audioContext.createMediaStreamSource(stream);
    // ... (process audio data)
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

### &#10022; Handling Cookies:
Cookies are small pieces of data stored on the user's computer by a web server as same as local storage.

```javascript
/* Setting Cookies */
document.cookie = 'name=Vel Murugan; expires=Thu, 31 Dec 2024 12:00:00 GMT';
/* Reading Cookies */
let cookies = document.cookie.split(';');
```

### &#10022; Other APIs:
- *Battery Status API:* Provides information about the device's battery status.
- *Vibration API:* Allows the device to vibrate.
- *Device Orientation API:* Provides information about the device's orientation.
- *Device Motion API:* Provides information about the device's acceleration and rotation.
- *Pointer Lock API:* Allows the user to lock the pointer to an element

---
[&#8682; To Top](#-web-apis)

[&#10094; Previous Topic](./json.md)

[&#8962; Goto Home Page](../README.md)
