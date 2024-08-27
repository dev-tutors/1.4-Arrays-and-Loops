### For Loops - Iterating Over Arrays

One of the most common tasks you'll perform with arrays is iterating over their elements—meaning, you go through each element in the array one by one. 

`for` loops are a powerful and straightforward way to do this. Let’s explore how `for` loops work and how they can help you efficiently access and manipulate elements in an array.

## Steps

### 1. Understanding the For Loop

A `for` loop is a control structure that allows you to repeat a block of code a certain number of times. When working with arrays, you can use a `for` loop to iterate through each element in the array, accessing or modifying the elements as needed.

### 2. Basic Structure of a For Loop

The basic syntax of a `for` loop looks like this:

```javascript
for (initialization; condition; increment) {
    // code to be executed in each iteration
}
```

- **Initialization:** This is where you start your loop, typically by declaring a counter variable (e.g., `let i = 0`).
- **Condition:** The loop continues as long as this condition is true (e.g., `i < array.length`).
- **Increment:** After each iteration, the counter is updated (e.g., `i++`).

### 3. Iterating Over an Array

To iterate over an array, you can combine the `for` loop with the array’s length property. Here’s how you can loop through an array of numbers and print each element:

```javascript
let numbers = [10, 20, 30, 40, 50];

for (let i = 0; i < numbers.length; i++) {
    console.log(numbers[i]);
}
```

### 4. Using For Loops to Modify Array Elements

You can also use `for` loops to modify elements in an array. For example, you can double the value of each element in an array of numbers:

```javascript
for (let i = 0; i < numbers.length; i++) {
    numbers[i] = numbers[i] * 2;
}

console.log(numbers); // Outputs: [20, 40, 60, 80, 100]
```

### 5. Summing Up Array Elements

Another common use of `for` loops is to calculate the sum of all elements in an array:

```javascript
let total = 0;

for (let i = 0; i < numbers.length; i++) {
    total += numbers[i];
}

console.log("Total sum: " + total);
```

### Full Code

<details>
<summary>Full Code</summary>

```javascript
let numbers = [10, 20, 30, 40, 50];

// Iterating over the array and printing each element
for (let i = 0; i < numbers.length; i++) {
    console.log(numbers[i]);
}

// Modifying the array elements by doubling their value
for (let i = 0; i < numbers.length; i++) {
    numbers[i] = numbers[i] * 2;
}

console.log(numbers); // Outputs: [20, 40, 60, 80, 100]

// Calculating the sum of all elements in the array
let total = 0;

for (let i = 0; i < numbers.length; i++) {
    total += numbers[i];
}

console.log("Total sum: " + total); // Outputs: Total sum: 300
```

</details>

## Explanation

- **Iteration:** The `for` loop is a versatile tool that allows you to iterate over an array's elements efficiently. By using the loop counter (`i`) as the array index, you can access and manipulate each element in the array.

- **Condition and Array Length:** The loop continues to run as long as the condition (`i < numbers.length`) is true. This ensures the loop iterates through every element in the array, regardless of its length.

- **Modifying Elements:** By using the `for` loop, you can easily modify each element in the array. In this example, each number in the array was doubled by multiplying it by `2`.

- **Summing Elements:** The `for` loop is also useful for accumulating values, such as summing up all the elements in an array.

## Important Notes

- **Avoid Hardcoding Array Length:** Always use `array.length` in your loop condition instead of hardcoding a specific number. This makes your loop adaptable to arrays of any length.

- **Infinite Loops:** Be careful to ensure your loop condition will eventually become false. Otherwise, you could create an infinite loop that crashes your program.

- **Efficiency:** `For` loops are efficient for processing arrays because they allow you to access and modify elements in a single pass through the array.

Using `for` loops to iterate over arrays is a fundamental skill in JavaScript. This is essential especially when you need to handle a wide range of tasks involving arrays, from simple data processing to more complex algorithms.