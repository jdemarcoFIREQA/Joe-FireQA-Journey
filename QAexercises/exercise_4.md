#Exercise 4: Boundary Value Analysis
- **Goal:** Practice testing the extreme limits of input fields (minimum, maximum, just below min, just above max).
- **Prompt:** Write test cases for a field that accepts an integer value for the **quantity of an item** with a **minimum of 1** *and* **a maximum of 99**.
- **Focus:** Testing the boundaries: 1, 99, 0, and 100.

|Scenario|Input Value|Given|When|Then|
|--------|-----------|-----|----|----|
|**Boundary Max (99)**|**99**|The user is viewing an item's page.|The user enters **99** in the **Quantity field** and clicks **"Add to Cart"**.|The item is successfully added to the cart with a quantity of **99**.|
|**Boundary Above Max (100)**|**100**|The user is viewing an item's page.|The user enters **100** in the **Quantity field** and clicks **"Add to Cart"**.|An **error message** appears: **"Maximum quantity per order is 99."**|
|**Boundary Min (1)**|**1**|The user is viewing an item's page.|The user enters **1** in the **Quantity field** and clicks **"Add to Cart"**.|The item is successfully added to the cart with a quantity of **1**.|
|**Boundary Below Min (0)**|**0**|The user is viewing an item's page.|The user enters **0** in the **Quantity field** and clicks **"Add to Cart"**.|An **error message** appears: **"Minimum quantity is 1."**|
