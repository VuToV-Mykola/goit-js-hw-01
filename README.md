# JavaScript Homework 01

## Task 1. Droid Orders

**File:** `task-1.js`

The repair droid sales station is ready to go, all that remains is to write the software for the sales department.

Declare the `makeTransaction` function, which expects two parameters:
- `quantity` — the first parameter, a number containing the number of ordered droids
- `pricePerDroid` — the second parameter, a number containing the cost of one droid

Add the code of the function so that it returns a string with a message about the purchase of repair droids:

`"You ordered <quantity> droids worth <totalPrice> credits!"`

Where:
- `<quantity>` is the number of droids ordered
- `<totalPrice>` is the total cost of the order (cost of all droids ordered)

### Test Code

Add the following code after your function declaration to check its correctness:

```javascript
console.log(makeTransaction(5, 3000)); // "You ordered 5 droids worth 15000 credits!"
console.log(makeTransaction(3, 1000)); // "You ordered 3 droids worth 3000 credits!"
console.log(makeTransaction(10, 500)); // "You ordered 10 droids worth 5000 credits!"
```

### Mentor Review Criteria

- Declared function `makeTransaction(quantity, pricePerDroid)`
- Calling `makeTransaction(5, 3000)` returns `"You ordered 5 droids worth 15000 credits!"`
- Calling `makeTransaction(3, 1000)` returns `"You ordered 3 droids worth 3000 credits!"`
- Calling `makeTransaction(10, 500)` returns `"You ordered 10 droids worth 5000 credits!"`
- All test results are output to the console
- Function works correctly with any valid arguments

## Task 2. Product Delivery

**File:** `task-2.js`

Declare the `getShippingMessage` function, which expects three parameters:
- `country` — the first parameter, a string containing the delivery country
- `price` — the second parameter, a number containing the total product cost
- `deliveryFee` — the third parameter, a number containing the delivery cost

Add the code of the function so that it returns a string with a message about product delivery:

`"Shipping to <country> will cost <totalPrice> credits"`

Where:
- `<country>` is the delivery country
- `<totalPrice>` is the total order cost (product cost + delivery cost)

### Test Code

Add the following code after your function declaration:

```javascript
console.log(getShippingMessage("Australia", 120, 50)); // "Shipping to Australia will cost 170 credits"
console.log(getShippingMessage("Germany", 80, 20)); // "Shipping to Germany will cost 100 credits"
console.log(getShippingMessage("Sweden", 100, 20)); // "Shipping to Sweden will cost 120 credits"
```

### Mentor Review Criteria

- Declared function `getShippingMessage(country, price, deliveryFee)`
- Calling `getShippingMessage("Australia", 120, 50)` returns `"Shipping to Australia will cost 170 credits"`
- Calling `getShippingMessage("Germany", 80, 20)` returns `"Shipping to Germany will cost 100 credits"`
- Calling `getShippingMessage("Sweden", 100, 20)` returns `"Shipping to Sweden will cost 120 credits"`
- Function works correctly with any valid arguments

## Task 3. Element Width

**File:** `task-3.js`

Declare the `getElementWidth` function, which expects three parameters:
- `content` — the first parameter, content width
- `padding` — the second parameter, horizontal padding value for each side
- `border` — the third parameter, border thickness value for each side

All parameter values will be strings in the format `Npx` where N is any number (integer or decimal).

Add the code of the function so that it returns a number — the total element width. When calculating the total width, consider that the `box-sizing` value equals `border-box`.

### Test Code

Add the following code after your function declaration:

```javascript
console.log(getElementWidth("50px", "8px", "4px")); // 74
console.log(getElementWidth("60px", "12px", "8.5px")); // 101
console.log(getElementWidth("200px", "0px", "0px")); // 200
```

### Mentor Review Criteria

- Declared function `getElementWidth(content, padding, border)`
- Calling `getElementWidth("50px", "8px", "4px")` returns number `74`
- Calling `getElementWidth("60px", "12px", "8.5px")` returns number `101`
- Calling `getElementWidth("200px", "0px", "0px")` returns number `200`
- Function works correctly with any valid arguments