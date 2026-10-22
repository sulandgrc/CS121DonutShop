# Donut Shop

## Topics

- Random number generation
- Conditional execution
- Scanner input

## Directions

Create a Java program that simulates purchasing donuts at a donut shop. Read the method descriptions below and add the methods to `DonutShop.java`. As you add each method, update the `main` method where indicated by the `TODO` comments.

**Starter code:** Add the starter-code link here.

### 1. Add a `getDonuts()` method

This method must:

- Take no parameters.
- Generate a random number of donuts to purchase between **6 and 30, inclusive**.
- Return the number of donuts purchased.

### 2. Add a `getCost()` method

This method must:

- Take no parameters.
- Randomly select a donut cost from three options: **$1.25**, **$1.75**, or **$2.50**.
- Return the cost of one donut.

To select the cost:

1. Use the `Random` class to construct a random number generator object.
2. Use its `nextInt()` method to generate an integer between **1 and 3, inclusive**.
3. Use the most efficient `if` structure to determine the cost:
   - If the random number is `1`, set the cost to `$1.25`.
   - If the random number is `2`, set the cost to `$1.75`.
   - If the random number is `3`, set the cost to `$2.50`.

### 3. Add a `getSubtotal(numDonuts, donutCost, discount)` method

This method must:

- Take three parameters:
  - `numDonuts`: The number of donuts purchased.
  - `donutCost`: The cost of each donut.
  - `discount`: The discount rate in decimal form, such as `0.25` for 25%.
- Return the amount owed after applying the discount and before adding sales tax.

### 4. Add a `printReceipt(subtotal)` method

This method must:

- Take the discounted subtotal as a parameter.
- Calculate sales tax as **10% of the subtotal**.
- Calculate the final total by adding sales tax to the subtotal.
- Print the customer's receipt to the console, including the subtotal, sales tax, and final total.
- Display monetary amounts with two decimal places.
- Return nothing (`void`).

### 5. Complete the `TODO` comments in `main`

Use `Scanner` to read the customer's discount in decimal form. Call your methods to generate the number of donuts, determine the cost per donut, calculate the discounted subtotal, and print the receipt.

## Sample Run

The number of donuts and cost per donut are randomly generated, so your results may vary.

```text
Enter your discount (0.0, 0.10, 0.25, etc): 0.25

You are going to buy 7 donuts!

Each donut will cost $1.25.

********** CUSTOMER RECEIPT **********
--------------------------------------
        Subtotal:         $6.56
        Sales Tax:        $0.66
--------------------------------------
TOTAL WITH SALES TAX:      $7.22
--------------------------------------
```
