### Challenge: 🔥 Find the Maximum Number in an Array

Ever wondered how to quickly find the highest number in a list? In this challenge, you’ll write a function that does just that! Let’s dive into finding the maximum value in an array.

## ⛳ Scenario

You have an array filled with numbers, and your task is to create a function that iterates through the array and returns the maximum number. If the array is empty, the function should return a message indicating that there are no numbers to compare.

### Example Inputs and Outputs

```javascript
// == Example 1 ==
// console.log(findMaxNumber([10, 25, 37, 45, 99])) = "The maximum number is 99"

// == Example 2 ==
// console.log(findMaxNumber([])) = "The array is empty. No maximum number to find."
```

## ✅ Task

1. **Create an Array of Numbers**

   - Define an array that contains at least 5 different numbers.

2. **Identify the Maximum Number**

   - Within your function, start by determining an initial value to compare against other numbers in the array.

3. **Iterate Through the Array**

   - Loop through the array, comparing each number to your initial value. Update your value if a larger number is found.

4. **Return the Result**
   - Once the loop is complete, return the largest number found. Display this result using `console.log()`.

## 💬 Quote of the day

"Success is the sum of small efforts, repeated day in and day out." — Robert Collier

## 🧠 Hints

<details> 
<summary>Hint 1</summary> 
Start your loop from the second element since the first element is already stored in `maxNumber`. 
</details> 
<br> 

<details> 
<summary>Hint 2</summary> 
Before starting the loop, make sure to handle the scenario where the array might be empty. </details> 
<br> 

<details> 
<summary>Hint 3</summary> 
Use an `if` statement inside the loop to update `maxNumber` whenever you encounter a larger number. </details>

## ⚡ Pseudocode Solution

<details>
<summary>Pseudocode</summary>

```
1. Create an array named numbers with at least 5 different numbers.

2. Write a function named findMaxNumber that accepts one parameter (the array).

3. Inside the function:
    a. Check if the array is empty. If it is, return "The array is empty. No maximum number to find."
    b. Initialize a variable maxNumber with the value of the first element in the array.
    c. Use a for loop to iterate through the array starting from the second element.
    d. Inside the loop, compare each element to maxNumber. If an element is greater than maxNumber, update maxNumber with this element.
    e. After the loop ends, return maxNumber as the maximum number in the array.

4. Test the function with different arrays to ensure it works correctly.
```

</details>
