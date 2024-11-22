## &#9873; Date and Time
JavaScript provides a rich set of built-in functions and objects to handle dates and times.

### &#9780; Overview:
1. [Creating Date Objects](#-creating-date-objects)
2. [Getting Date and Time Components](#-getting-date-and-time-components)
3. [Formatting Dates and Times](#-formatting-dates-and-times)
4. [Time Differences](#-time-differences)
5. [Time Zones](#-time-zones)
6. [Setting a Time](#-setting-a-time)

### &#10022; Creating Date Objects:
To create a `Date` object to represent a specific instant in time.

*Example:*
```javascript
// Current time
const now = new Date();
console.log(now); // Output: Fri Nov 22 2024 17:02:07 GMT+0530 (India Standard Time) (example)

// Specific date and time
const specificDate = new Date(2024, 10, 22, 16, 59, 0); // Month is 0-indexed (Starts January with 0)
console.log(specificDate); // Output: Fri Nov 22 2024 16:59:00 GMT+0530 (India Standard Time) (example)
```

### &#10022; Getting Date and Time Components:
To get various components from a `Date` object.

*Example:*
```javascript
// Current time
const now = new Date();

// Various date components
const year = now.getFullYear();
const month = now.getMonth() + 1; // Months are 0-indexed
const date = now.getDate();
const day = now.getDay(); // Day of the week (0-6, 0 is Sunday)
const hours = now.getHours();
const minutes = now.getMinutes();
const seconds = now.getSeconds();
const milliSeconds = now.getMilliseconds();

console.log(`Date: ${date}/${month}/${year} Time: ${hours}:${minutes}:${seconds}`);
// Output: Date: 22/11/2024 Time: 17:5:46 (example)
```

### &#10022; Formatting Dates and Times:
To format dates and times using the `toLocaleString()` and `toLocaleTimeString()` methods.

*Example:*
```javascript
// Current time
const now = new Date();

const formattedDate = now.toLocaleDateString();
const formattedTime = now.toLocaleTimeString();
const formattedDateTime = now.toLocaleString('en-IN', {
    year: 'numeric',
    month: 'long',
    day: 'numeric',
    hour: 'numeric',
    minute: 'numeric',
    second: 'numeric',
    timeZoneName: 'short'
});

console.log(formattedDate); // Output: 11/22/2024 (example)
console.log(formattedTime); // Output: 5:10:11 PM (example)
console.log(formattedDateTime); // Output: 22 November 2024 at 5:08:57 pm IST (example)
```

*Example:* Custom Formatting
```javascript
let now = new Date();
let options = { year: 'numeric', month: 'long', day: 'numeric' };
let formattedDate = new Intl.DateTimeFormat('en-US', options).format(now);
console.log(formattedDate); // Output: November 22, 2024 (example)
```

### &#10022; Time Differences:
To calculate the difference between two given dates using the `getTime()` method, which returns the number of milliseconds since the Unix epoch.

```javascript
const date1 = new Date(2024, 11, 1);
const date2 = new Date(2025, 0, 1);

const timeDifference = date2.getTime() - date1.getTime();
const daysDifference = timeDifference / (1000 * 60 * 60 * 24);

console.log(timeDifference); // Output: 2678400000
console.log(daysDifference); // Output: 31
```

### &#10022; Time Zones:
To work with different time zones using the `getTimezoneOffset()` method.

```javascript
const offset = now.getTimezoneOffset(); // Minutes offset from UTC
```

To create a `Date` object in a specific time zone, by using the `toLocaleString()` method with appropriate options.

### &#10022; Setting a Time:
To set a specific components of a `Date` object.

```javascript
// Current time
const date = new Date();

date.setFullYear(2025);
date.setMonth(0); // January
date.setDate(1);
date.setHours(12);
date.setMinutes(0);
date.setSeconds(0);

console.log(date); // Output: Wed Jan 01 2025 12:00:00 GMT+0530 (India Standard Time)
```

*Example:* Short way to specify a date
```javascript
let newYear = new Date(2025, 0, 31); // Month is 0-indexed (January is 0)
console.log(newYear); // Output: Fri Jan 31 2025 00:00:00 GMT+0530 (India Standard Time)
```

---
[&#8682; To Top](#-date-and-time)

[&#10094; Previous Topic](./functions.md) &emsp; [Next Topic &#10095;](./dom-manipulation.md)

[&#8962; Goto Home Page](../README.md)