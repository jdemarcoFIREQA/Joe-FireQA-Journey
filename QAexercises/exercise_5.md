#Exercise 5: API-Level Testing (CRUD)
- **Goal:** Practice translating functional requirements into test cases for RESTful API endpoint using the Given-When-Then format, focusing on HTTP status codes and response bodies.
- **Feature:** A simple **Notes** API endpoint (/api/notes) that allows creating and retrieving notes.
- **Focus:** API Interactions, status codes, and data verification.

|Scenario|Given|When|Then|
|--------|-----|----|----|
|**Successful Note Creation (POST)**|The user has a **valid authentication token.**|A **POST** request is sent to */api/notes* with a **valid JSON body** containing a *title* and *content*.|The API responds with an **HTTP 201 Created** status code, and the **response body** contains the **newly created Note object**, including a unique *note_id*.|
|**Invalid Input (POST)**|The user has a **valid authentication token**.|A **POST** request is sent to */api/notes* with an **invalid JSON body** where the required *title* field is missing.|The API responds with an **HTTP 400 Bad Request** status code, and the **response body** contains a clear error message indicating the missing field.|
|**Successful Note Retrieval (GET)**|A **Note (ID: 123)** already exists in the database.|A **GET** request is sent to */api/notes/123*.|The API responds with an *HTTP 200 OK* status code, and **the response body** contains the data for **Note 123** (matching the title and content stored).|
|**Note Not Found (GET)**|**No Note** with **ID: 999** exists in the database.|A **GET** request is sent to */api/notes/999*.|The API responds with an *HTTP 404 Not Found* status code, and the **response body** may be empty or contain a "Resource not found" message.|
