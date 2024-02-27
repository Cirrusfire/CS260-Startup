# Web Development Midterm Study Guide

## HTML (Hypertext Markup Language)
- HTML is the standard markup language for creating web pages.
- It defines the structure and content of a web page using elements and tags.

### Commonly Used Tags:
- `<div>`: Defines a division or a section.
- `<p>`: Defines a paragraph.
- `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`: Define headings of different sizes.
- `<a>`: Defines a hyperlink.
- `<img>`: Defines an image.
- `<ul>`: Defines an unordered list.
- `<li>`: Defines a list item.
- `<ol>`: Defines an ordered (numbered) list.

### Flexbox Examples:
- Basic Flex Container with Items:
  ```html
  <div style="display: flex;">
      <div style="background-color: red; width: 100px; height: 100px;"></div>
      <div style="background-color: blue; width: 100px; height: 100px;"></div>
      <div style="background-color: green; width: 100px; height: 100px;"></div>
  </div>
  
- Flex Container with Items Aligned Horizontally:
  ```html
  <div style="display: flex; justify-content: space-between;">
    <div style="background-color: red; width: 100px; height: 100px;"></div>
    <div style="background-color: blue; width: 100px; height: 100px;"></div>
    <div style="background-color: green; width: 100px; height: 100px;"></div>
  </div>

- Flex Container with Items Aligned Vertically:
  ```html
  <div style="display: flex; flex-direction: column;">
    <div style="background-color: red; width: 100px; height: 100px;"></div>
    <div style="background-color: blue; width: 100px; height: 100px;"></div>
    <div style="background-color: green; width: 100px; height: 100px;"></div>
  </div>

- Flex Container with Items Wrapped:
  ```html
  <div style="display: flex; flex-wrap: wrap;">
    <div style="background-color: red; width: 100px; height: 100px;"></div>
    <div style="background-color: blue; width: 100px; height: 100px;"></div>
    <div style="background-color: green; width: 100px; height: 100px;"></div>
  </div>

- Flex Container with Items Justified and Aligned:
  ```html
  <div style="display: flex; justify-content: space-between; align-items: center;">
    <div style="background-color: red; width: 100px; height: 100px;"></div>
    <div style="background-color: blue; width: 100px; height: 150px;"></div>
    <div style="background-color: green; width: 100px; height: 80px;"></div>
  </div>

- Flex Container with Items Ordered:
  ```html
  <div style="display: flex;">
    <div style="background-color: red; width: 100px; height: 100px;"></div>
    <div style="background-color: blue; width: 100px; height: 100px; order: 3;"></div>
    <div style="background-color: green; width: 100px; height: 100px; order: 2;"></div>
    <div style="background-color: yellow; width: 100px; height: 100px; order: 1;"></div>
  </div>



## CSS (Cascading Style Sheets)
- CSS is used to style the HTML elements, controlling their layout, appearance, and presentation.
- Basic properties include styling attributes like color, font size, background color, margin, padding, etc.

### Selectors:
- Class selector: Targets elements with a specific class attribute.
- ID selector: Targets a specific element with a unique ID attribute.

#### Selectors Example:
  ```CSS
    /* Style for class header */
  .header {
      font-size: 24px;
      color: blue;
  }
  
  /* Style for ID header */
  #header {
      font-weight: bold;
      text-decoration: underline;
  }
```

### Box Model:
![CSS Box Model](https://www.washington.edu/accesscomputing/webd2/student/unit3/images/boxmodel.gif)

## JavaScript
- JavaScript adds interactivity and dynamic behavior to web pages.
- Basic statements include variables, loops, conditionals, etc.
- Functions are blocks of reusable code.
- Objects are containers for named values (properties) and methods.
- Arrays store multiple values.
- Higher-order functions (map, reduce, forEach, filter) operate on other functions.
- Asynchronous JavaScript includes Promises, async/await.
- The DOM (Document Object Model) of a web page is a programming interface that represents the web page as a tree of objects, allowing JavaScript to access and manipulate the content and structure of the web page dynamically.
- Fetch API is used to make HTTP requests.
- JSON (JavaScript Object Notation) is a lightweight data interchange format used to transmit data between a server and a web application.

### JavaScript Examples:
- Basic for loop:
  ```javascript
  for (let i = 0; i < 5; i++) {
      console.log(i);
  }
- while loop:
  ```javascript
  let i = 0;
  while (i < 5) {
    console.log(i);
    i++;
  }
- example of fetch() from an API:
  ```javascript
  fetch('https://api.example.com/data')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error('Error fetching data:', error));
- Changing text color of all <p> elements with ID "header" to red:
  ```javascript
  const headerParagraphs = document.querySelectorAll('p#header');
  headerParagraphs.forEach(paragraph => {
      paragraph.style.color = 'red';
  });
- Creating javascript object:
  ```javascript
  const myObject = { key1: value1, key2: value2 };
- Accessing properties of javascript object:
  ```javascript
  const myObject = { name: "John", age: 30 };
  console.log(myObject.name); // Output: John
  console.log(myObject["age"]); // Output: 30
- Adding a new property to a JavaScript object at runtime:
  ```javascript
  const myObject = {};
  myObject.newProperty = "value";
- Using forEach() to execute a function on each element in an array:
  ```javascript
  const numbers = [1, 2, 3, 4, 5];
  numbers.forEach(number => console.log(number));
- Using filter() to create a new array with elements passing a test:
  ```javascript
  const numbers = [1, 2, 3, 4, 5];
  const evenNumbers = numbers.filter(number => number % 2 === 0);
  console.log(evenNumbers); // Output: [2, 4]
- Using map() to create a new array with results of a function on each element:
  ```javascript
  const numbers = [1, 2, 3, 4, 5];
  const doubledNumbers = numbers.map(number => number * 2);
  console.log(doubledNumbers); // Output: [2, 4, 6, 8, 10]
- Using Javascript to change the HTML of an element:
  ```javascript
  document.getElementById("myElement").innerHTML = "New content";

