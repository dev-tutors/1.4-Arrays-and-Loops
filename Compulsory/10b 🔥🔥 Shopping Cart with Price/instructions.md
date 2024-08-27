### Challenge: 🔥🔥 Shopping Cart with Price

Now that you're familiar with building a shopping cart, let's take it up a notch! In this level 2 challenge, you'll enhance your shopping cart by adding prices to each item. This will allow you to track not just what’s in the cart, but also how much everything costs, and calculate the total price of all the items.

## ⛳ Scenario

You’re building an advanced shopping cart where the user will input how many items they want to add, then enter both the name and price of each item. The cart will store these items and their prices, and once the user is done, the cart’s contents will be displayed along with the total cost.

### Example Inputs and Outputs

```javascript
// == Example 1 ==
// Please enter the number of items to add to cart: 3
// Enter item 1: Apple
// Enter price for Apple: 1.5
// Enter item 2: Bread
// Enter price for Bread: 2.0
// Enter item 3: Milk
// Enter price for Milk: 1.2
// Output: 
// "Your cart contains:
// Apple - $1.5
// Bread - $2.0
// Milk - $1.2
// Total Price: $4.7"

// == Example 2 ==
// Please enter the number of items to add to cart: 2
// Enter item 1: Chocolate
// Enter price for Chocolate: 3.5
// Enter item 2: Juice
// Enter price for Juice: 2.5
// Output: 
// "Your cart contains:
// Chocolate - $3.5
// Juice - $2.5
// Total Price: $6.0"
```

## ✅ Task

1. **Collecting Item Details**
   - Ask the user to input the number of items they wish to add to their cart.
   - Gather the name and price for each item, one by one.

2. **Store Items and Prices**
   - Save each item’s name and its price in a way that they can be easily accessed later.

3. **Calculate the Total Cost**
   - As the user inputs the prices, keep a running total of the combined price of all items.

4. **Display the Final Cart**
   - Once all items have been added, show a list of all items along with their prices, and display the total price at the end.

## 💬 Quote of the day

"The price of anything is the amount of life you exchange for it." — Henry David Thoreau

## 🧠 Hints

For the best learning experience, try solving the challenge using just the requirements and understanding the inputs and outputs. Refer to the hints only if needed.

<details>
<summary>Hint 1</summary>
Consider whether you want to use separate arrays for the item names and prices, or combine them into a single structure.
</details>

<br>

<details>
<summary>Hint 2</summary>
You might need to convert the price input from a string to a number before performing any calculations.
</details>

<br>

<details>
<summary>Hint 3</summary>
To display each item on a new line, you can use `\n` in your output formatting.
</details>

## ⚡ Pseudocode Solution

<details>
<summary>Pseudocode</summary>

```
1. Use prompt() to ask the user how many items they want to add to the cart. Store this in a variable.

2. Create an empty array named cart to store the items.
   Create a variable named totalPrice initialized to 0.

3. Write a for loop that runs for the number of items the user specified.

4. Inside the loop:
    a. Use prompt() to ask for the item name.
    b. Use prompt() to ask for the item price.
    c. Convert the price from a string to a number.
    d. Push the item and its price as a string into the cart array.
    e. Add the price to totalPrice.

5. After the loop, use console.log() to display the contents of the cart with prices, each on a new line.
   Use console.log() to display the total price of all items.
```

</details>
