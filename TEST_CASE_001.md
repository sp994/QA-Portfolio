Test Case: Verify Shopping Cart Quantity Update

**Test Case ID:** TC-001  
**Priority:** High  
**Feature:** Shopping Cart  

---

### Description
Verify that a user can manually update the quantity of a product in the shopping cart and that the total price updates correctly.

### Preconditions
* User is logged into the e-commerce site.
* At least one item is already in the shopping cart.

### Test Steps
1. Navigate to the **Shopping Cart** page.
2. Locate the **Quantity** input field for an item.
3. Delete the current value and enter `5`.
4. Press the **Enter** key or click the **Update** button.
5. Observe the quantity value and the subtotal.

### Expected Result
* The quantity field should display `5`.
* The subtotal should recalculate correctly (Unit Price x 5).
* No error messages should appear.

### Post-conditions
* The cart reflects the updated quantity for the remainder of the session.
