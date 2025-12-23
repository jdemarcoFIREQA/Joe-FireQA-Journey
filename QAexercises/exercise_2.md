#Exercise 2: Negative Testing (Error Paths)

**Goal:** Practice identifying common failure points and documenting expected error handling. 
**Prompt:** Write three test cases for a user trying to **register** a new account.
**Focus:** Input validation, boundary conditions, and error message accuracy. 

|Scenario|Given|When|Then|
|--------|-----|----|----|
|**Invalid Email Format**|The user is on the **Registration Page**.|The user enters a **password** and a **Username**, but uses an email address without an "@" symbol (e.g., testexample.com), and clicks "Register".|An **inline error message** appears next to the email field: "Please enter a valid email address."|
|**Password Too Short**|The user is on the **Registration Page**.|The user enters a **valid email** and Username, but a **password** with fewer than 8 characters (e.g., pass123), and clicks **"Register"**.|The system **prevents registration** and displays the error: **"Password must be at least 8 characters long."**|
|**Existing Username**|The user is on the **Registration Page**.|The user enters a **valid email** and **password**, but a **Username that is already taken** (e.g., *johndoe*), and clicks **"Register"**.|The system **prevents registration** and displays the error: **"This username is already in use. Please choose another."**|
