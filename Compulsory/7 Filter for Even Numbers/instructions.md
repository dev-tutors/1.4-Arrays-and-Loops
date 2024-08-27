### Filtering Even Numbers Using a For Loop

Filtering specific elements from an array is a common task in programming. In this lesson, you’ll learn how to filter even numbers from an array using a traditional `for` loop. This method allows you to manually control the filtering process, giving you a deeper understanding of how arrays and loops work together.

## Steps

### 1. Define the Arrays

Start by creating an array that contains the numbers you want to filter. Then, define an empty array where the even numbers will be stored.

```javascript
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
let evenNumbers = [];
```

### 2. Use a `for` Loop to Filter Even Numbers

Now that you've set up your arrays, use a `for` loop to iterate through each number in the `numbers` array. Inside the loop, you'll check if the current number is even.

```javascript
for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] % 2 === 0) {
        evenNumbers.push(numbers[i]);
    }
}
```

### 3. Display the Result

After filtering the even numbers, use `console.log()` to display the contents of the `evenNumbers` array.

```javascript
console.log(evenNumbers); // Outputs: [2, 4, 6, 8, 10]
```

### Full Code

<details>
<summary>Full Code</summary>

```javascript
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
let evenNumbers = [];

// Using a for loop to filter even numbers
for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] % 2 === 0) {
        evenNumbers.push(numbers[i]);
    }
}

console.log(evenNumbers); // Outputs: [2, 4, 6, 8, 10]
```

</details>

## Explanation

- **Iteration:** The `for` loop goes through each element in the `numbers` array, one by one.
- **Condition:** The `if` statement checks whether the current number is even by using the modulus operator (`%`). If the result is `0`, the number is even.
- **Adding to New Array:** When a number is found to be even, it’s added to the `evenNumbers` array using `push()`.

## Important Notes

- **Modulus Operator (`%`):** The modulus operator is a crucial tool in checking for even numbers. It returns the remainder of a division operation, which is `0` for even numbers.

- **Flexibility:** You can modify the condition inside the `if` statement to filter out numbers based on different criteria (e.g., odd numbers, numbers greater than a certain value).
