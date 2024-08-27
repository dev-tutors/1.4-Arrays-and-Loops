### Working with `splice()` and `slice()` Methods

When working with arrays, you'll often need to remove, replace, or extract elements. The `splice()` and `slice()` methods in JavaScript are perfect for these tasks.

In this lesson, we'll focus on how to use these two powerful tools effectively. Since we're on the topic of slicing, let's use emojis instead of just words for this lesson just to make it more memorable 😉

## Steps

### 1. Understanding the `splice()` Method

The `splice()` method allows you to add, remove, or replace elements in an array at a specific position. This method modifies the original array.

**Syntax:**

```javascript
array.splice(start, deleteCount, item1, item2, ...);
```

- **start:** The index at which to start changing the array.
- **deleteCount:** The number of elements to remove (optional).
- **item1, item2, ...:** The elements to add to the array (optional).

#### a. Removing Elements

You can remove one or more elements from an array using `splice()` by specifying the starting index and the number of elements to remove:

```javascript
let fruits = ["🍎", "🍌", "🍊", "🍉"];
let removedItems = fruits.splice(1, 2); // Removes 2 elements starting from index 1
console.log(fruits); // Outputs: ["🍎", "🍉"]
console.log(removedItems); // Outputs: ["🍌", "🍊"]
```

#### b. Replacing Elements

You can also replace elements by specifying the elements to add after removing the specified number of elements:

```javascript
fruits.splice(1, 1, "🍇", "🍍"); // Replaces 1 element at index 1 with "🍇" and "🍍"
console.log(fruits); // Outputs: ["🍎", "🍇", "🍍", "🍉"]
```

### 2. Understanding the `slice()` Method

The `slice()` method returns a new array containing a portion of the original array, starting from a specified index and ending at another index (not inclusive). The original array remains unchanged.

**Syntax:**

```javascript
array.slice(start, end);
```

- **start:** The index at which to begin extraction (inclusive).
- **end:** The index at which to end extraction (exclusive). If omitted, extraction continues to the end of the array.

#### a. Extracting a Portion of an Array

You can extract a portion of an array using `slice()` without modifying the original array:

```javascript
let fruits = ["🍎", "🍌", "🍊", "🍉"];
let citrus = fruits.slice(1, 3); // Extracts elements from index 1 to 2 (not including index 3)
console.log(citrus); // Outputs: ["🍌", "🍊"]
console.log(fruits); // Outputs: ["🍎", "🍌", "🍊", "🍉"]
```

### Full Code

<details>
<summary>Full Code</summary>

```javascript
// Using splice() to remove and replace elements
let fruits = ["🍎", "🍌", "🍊", "🍉"];
let removedItems = fruits.splice(1, 2); // Removes 2 elements starting from index 1
console.log(fruits); // Outputs: ["🍎", "🍉"]
console.log(removedItems); // Outputs: ["🍌", "🍊"]

fruits.splice(1, 1, "🍇", "🍍"); // Replaces 1 element at index 1 with "🍇" and "🍍"
console.log(fruits); // Outputs: ["🍎", "🍇", "🍍", "🍉"]

// Using slice() to extract a portion of an array
let citrus = fruits.slice(1, 3); // Extracts elements from index 1 to 2 (not including index 3)
console.log(citrus); // Outputs: ["🍇", "🍍"]
console.log(fruits); // Outputs: ["🍎", "🍇", "🍍", "🍉"]
```

</details>

## Explanation

- **`splice()` Method:** The `splice()` method is versatile for removing, replacing, or adding elements to an array. It directly modifies the original array and returns an array of removed elements.

- **`slice()` Method:** The `slice()` method is useful for creating a new array from a portion of the original array. It does not alter the original array but provides a subset of its elements.

## Important Notes
- **Splicing and Slicing:** `splice()` is a powerful method that allows you to modify the content of an array by removing, replacing, or adding elements at any position. `slice()` is useful for extracting a portion of an array without altering the original.

- **Mutability:** `splice()` changes the original array, so be cautious when using it if you need to retain the original data. `slice()` is non-destructive and leaves the original array unchanged.

- **Return Values:** `splice()` returns an array of the removed elements, while `slice()` returns a new array containing the specified portion of the original array.

- **Indexes:** Both methods rely heavily on accurate indexing, so ensure that you are familiar with how array indices work (starting from 0).

## How to Use Documentation

To fully understand and leverage methods like `splice()` and `slice()`, it’s important to be comfortable using documentation. Let’s explore how to navigate the documentation:

### Documentation Resources:
- [W3Schools: splice() Method](https://www.w3schools.com/jsref/jsref_splice.asp)
- [W3Schools: slice() Method](https://www.w3schools.com/jsref/jsref_slice_array.asp)

Open one of the links and let's go through on how to use the learning resource effectively 💪! These are the 5 things you want to watch out for:

### 1. Description
- Read the description to understand what the method does.

### 2. Syntax
- Pay close attention to the syntax. Identify the required parameters and their positions.

### 3. Parameters
- Parameters are the inputs the method accepts. Documentation will tell you which parameters are required and which are optional.

### 4. Return Value
- Check what the method returns. This will help you understand what to expect after using the method.

### 5. Examples
- Review examples to see how the method is used in practice. Try running these examples on your own.

Mastering `splice()` and `slice()` gives you powerful tools for array manipulation, but the **real skill** that sets great developers apart is knowing how to **read and understand documentation**.

While ChatGPT is a fantastic resource, there are times—especially when working with internal tools or custom libraries—where you'll need to rely on your ability to navigate documentation.

This skill isn't just nice to have; it's **essential**. It's what separates a good developer from a great one, allowing you to solve problems independently and adapt to new challenges.