### Challenge: 🔥Find a Movie by Index

Imagine you have a list of your all-time favorite movies, and you want to quickly find out which movie is at a specific position in the list. In this challenge, you'll create a function that does just that!

## ⛳ Scenario

You have an array that stores your favorite movies in a specific order. Your task is to create a function that takes an index as an argument and returns the movie at that index. However, if the index is out of bounds (i.e., it doesn’t exist in the array), the function should return a message saying the index is invalid.

### Example Inputs and Outputs

```javascript
// == Example 1 ==
// console.log(getMovieByIndex(2)) = "The movie at index 2 is 'Inception'"

// == Example 2 ==
// console.log(getMovieByIndex(5)) = "Invalid index. Please provide a valid index."
```

## ✅ Task

1. **Create an Array of Favorite Movies**
   - Start by creating an array that contains at least 4 of your favorite movies.

2. **Write a Function to Find the Movie by Index**
   - The function should take one parameter (the index) and return the movie at that index.
   - If the index is invalid (either negative or greater than the array length), return an appropriate message.

## 💬 Quote of the day

"Every problem has a solution; sometimes you just have to think outside the box." — Anonymous

## 🧠 Hints

For the best learning experience, try solving the challenge using just the requirements and understanding the inputs and outputs. Refer to the hints only if needed.

<details>
<summary>Hint 1</summary>
Remember that arrays in JavaScript are zero-indexed, meaning the first element is at index `0`.
</details>

<br>

<details>
<summary>Hint 2</summary>
Use an `if` statement to check if the index is within the valid range before trying to access the movie.
</details>

<br>

<details>
<summary>Hint 3</summary>
The length of the array can help you determine the valid range for indices.
</details>

## ⚡ Pseudocode Solution

<details>
<summary>Pseudocode</summary>

```
1. Create an array named favoriteMovies with at least 4 movie titles.

2. Write a function named getMovieByIndex that accepts one parameter (index).

3. Inside the function:
    a. Check if the index is valid (i.e., greater than or equal to 0 and less than the length of the array).
    b. If valid, return the movie at the given index.
    c. If not valid, return a message saying "Invalid index. Please provide a valid index."

4. Test the function with different index values to ensure it works correctly.
```

</details>