### Challenge: 🔥 Build Your Shopping Cart

Ready to build a simple shopping cart? In this challenge, you’ll create a shopping cart simulation where users can add items and see everything they’ve added. Let’s dive in!

## ⛳ Scenario

You’re creating a basic shopping cart where the user will input how many items they want to add, then enter the name of each item. The cart will store these items in an array, and once the user is done, the cart’s contents will be displayed.

### Example Inputs and Outputs

```javascript
// == Example 1 ==
// Please enter the number of items to add to cart: 3
// Enter item 1: Apple
// Enter item 2: Bread
// Enter item 3: Milk
// "Your cart contains: Apple, Bread, Milk"

// == Example 2 ==
// Please enter the number of items to add to cart: 2
// Enter item 1: Chocolate
// Enter item 2: Juice
// "Your cart contains: Chocolate, Juice"
```

## ✅ Task

1. **Collect the Number of Items**
    
   Ask the user how many items they want to add to their cart.

2. **Set Up the Shopping Cart**
   
   Create a structure to store the items as the user adds them.

3. **Add Items to the Cart**
   
   Loop through, allowing the user to input the name of each item.

4. **Display the Cart Contents**
   
   After all items have been added, display the full list of items in the cart.

## 💬 Quote of the day

"The only way to do great work is to love what you do." — Steve Jobs

## 🧠 Hints

For the best learning experience, try solving the challenge using just the requirements and understanding the inputs and outputs. Refer to the hints only if needed.

<details>
<summary>Hint 1</summary>
Think about how you will store each item in the cart as the user adds them.
</details>

<br>

<details>
<summary>Hint 2</summary>
Consider using a method that allows you to add each item to the cart.
</details>

<br>

<details>
<summary>Hint 3</summary>
Use a method to combine all the items into a single string for display.
</details>

## ⚡ Pseudocode Solution

<details>
<summary>Pseudocode</summary>

```
1. Use prompt() to ask the user how many items they want to add to the cart. Store this in a variable.

2. Create an empty array named cart to store the items.

3. Write a for loop that runs for the number of items the user specified.

4. Inside the loop:
    a. Use prompt() to ask for the item name.
    b. Push the item into the cart array.

5. After the loop, use console.log(cart.join(", ")) to display the contents of the cart as a single string.
```

</details>