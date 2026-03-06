# Bug Report: Quantity Logic Error

## Project Context
**Industry:** Global E-commerce Platform  
**Testing Type:** Functional Regression Testing (via uTest)

---

### Description
During functional testing of a retail checkout flow, I identified a logic error where the quantity input field fails to retain user input when the Enter key is pressed.

### Steps to Reproduce
1. Navigate to a product detail page on the **[Client Site]**.
2. Add a product to the cart and proceed to the **Shopping Cart page**.
3. Manually enter `10` into the **Quantity** input field.
4. Press the **Enter** key.
5. Observe the quantity value.
6. Click back into the field and press **Enter** again to confirm the pattern.

### Expected Result
The quantity should remain at the user-defined value (`10`) and update the subtotal accordingly.

### Actual Result
The quantity decrements by 1 (changing from `10` to `9`) every time the Enter key is pressed.

// Developer Fix: Stopped auto-decrement on Enter key.

FIXED: Developer adjusted the event listener to ignore the Enter key in the quantity field.
