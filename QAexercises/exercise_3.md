#Exercise 3: State-Dependent Testing (Prerequisites)

- **Goal:** Practice defining complex preconditions (the *Given*) step) that involve prior actions or data states.
- **Prompt:** Write a test case for a user attempting to **purchase an item** from an e-commerce site.
- **Focus:** Ensuring the *Given* sets up the necessary context (e.g., an item in the cart, payment details saved).

  |Scenario|Given|When|Then|
  |--------|-----|----|----|
  |**Successful Checkout**|The user is **logged in**, has a **valid credit card** saved, and their **shopping cart contains 2 items** (Item A and Item B).|The user navigates to the **Checkout page, confirms the shipping address,** selects the **saved credit card**, and clicks **"Place Order"**.|The system displays an **"Order Confirmed"** message, the user receives an **order confirmation email**, and the **shopping cart is empty**.|
  
