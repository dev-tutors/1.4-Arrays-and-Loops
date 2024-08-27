### Common Array Methods

Arrays in JavaScript come with a set of built-in methods that make it easier to work with collections of data. These methods allow you to add, search, and manipulate elements within an array efficiently. 

Let’s explore some of the most commonly used array methods that will help you handle arrays like a pro!

## Steps

### 1. Adding Elements to an Array

**`push()` Method**

The `push()` method adds one or more elements to the end of an array. It’s a quick way to grow your array dynamically:

```javascript
let fruits = ["Apple", "Banana"];
fruits.push("Orange");
console.log(fruits); // Outputs: ["Apple", "Banana", "Orange"]
```

**`unshift()` Method**

The `unshift()` method adds one or more elements to the beginning of an array:

```javascript
fruits.unshift("Mango");
console.log(fruits); // Outputs: ["Mango", "Apple", "Banana", "Orange"]
```

### 2. Removing Elements from an Array

**`pop()` Method**

The `pop()` method removes the last element from an array and returns that element:

```javascript
let lastFruit = fruits.pop();
console.log(lastFruit); // Outputs: Orange
console.log(fruits);    // Outputs: ["Mango", "Apple", "Banana"]
```

**`shift()` Method**

The `shift()` method removes the first element from an array and returns that element:

```javascript
let firstFruit = fruits.shift();
console.log(firstFruit); // Outputs: Mango
console.log(fruits);     // Outputs: ["Apple", "Banana"]
```

### 3. Searching for Elements in an Array

**`indexOf()` Method**

The `indexOf()` method searches the array for a specific element and returns its first index. If the element is not found, it returns `-1`:

```javascript
let position = fruits.indexOf("Banana");
console.log(position); // Outputs: 1

let notFound = fruits.indexOf("Pineapple");
console.log(notFound); // Outputs: -1
```

**`includes()` Method**

The `includes()` method checks if an array contains a certain element, returning `true` or `false`:

```javascript
let hasApple = fruits.includes("Apple");
console.log(hasApple); // Outputs: true

let hasPineapple = fruits.includes("Pineapple");
console.log(hasPineapple); // Outputs: false
```

### Full Code

<details>
<summary>Full Code</summary>

```javascript
let fruits = ["Apple", "Banana"];

// Adding elements
fruits.push("Orange");
console.log(fruits); // Outputs: ["Apple", "Banana", "Orange"]

fruits.unshift("Mango");
console.log(fruits); // Outputs: ["Mango", "Apple", "Banana", "Orange"]

// Removing elements
let lastFruit = fruits.pop();
console.log(lastFruit); // Outputs: Orange
console.log(fruits);    // Outputs: ["Mango", "Apple", "Banana"]

let firstFruit = fruits.shift();
console.log(firstFruit); // Outputs: Mango
console.log(fruits);     // Outputs: ["Apple", "Banana"]

// Searching elements
let position = fruits.indexOf("Banana");
console.log(position); // Outputs: 1

let hasApple = fruits.includes("Apple");
console.log(hasApple); // Outputs: true
```
</details>

## Explanation

- **Adding and Removing Elements:** The `push()`, `pop()`, `unshift()`, and `shift()` methods make it easy to add or remove elements from the beginning or end of an array, helping you manage the size and content of your arrays dynamically.

- **Searching Elements:** `indexOf()` and `includes()` are handy for finding specific elements in an array, whether you need the index or just need to check for its presence.

## Important Notes

- **Modifying the Original Array:** Methods like `push()`, `pop()`, `shift()` modify the original array. Be cautious when using them if you need to preserve the original data.

- **Return Values:** Many array methods return values that you can use immediately. For example, `pop()` returns the removed element. Make sure to use these return values effectively.

- **Chaining Methods:** 
    - You can chain methods together to perform multiple operations in a single line. 
    - For example: `fruits.push("Orange").pop();` (This adds "Orange" to the end of the array and then immediately removes it. 
    - While chaining these methods may not always be common, it’s a good concept to understand for more complex operations.)

These common array methods are essential tools for working with lists of data in JavaScript. Mastering these methods will help you manipulate arrays with ease and handle a wide range of programming tasks. 

Keep experimenting with these methods in different scenarios to build your confidence!