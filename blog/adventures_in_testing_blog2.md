# Blog post 2: Test Case Triage: Anatomy of a Great Test Case

## Introduction

A test case is the fundamental building block of organized testing. It's not just a set of instructions; it's a piece of documentation that communicates exactly what you intend to verify. This blog breaks down the anatomy of a truly effective test case and introduces the concept of test triage.

## Key Components of an Effective Test Case

A high-quality test case is atomic, reusable, and easy to follow. It typically contains these core elements:

1.  **ID/Title:** A unique identifier (TC-001) and a clear, concise title (e.g., "Verify successful login with valid credentials").
2.  **Summary/Objective:** What is the specific goal of this test? (e.g., To ensure the authentication mechanism works as designed).
3.  **Preconditions:** What must be true before the test can be executed? (e.g., A user account must be registered and confirmed; the application server must be running).
4.  **Test Data:** The specific data inputs needed (e.g., Username: `testuser@example.com`, Password: `Password123!`).
5.  **Steps to Execute:** The sequence of actions the tester must perform. These must be detailed, singular actions.
6.  **Expected Result:** The observable outcome if the system works correctly. This must be unambiguous.
7.  **Status/Result:** The outcome of the execution (Pass, Fail, Blocked, N/A).

## Writing Clear and Actionable Steps

Clarity is paramount. Vague steps lead to inconsistent results and "flaky" tests.

| Poor Step | Good Step | Why it's better |
| :--- | :--- | :--- |
| Go to the login page. | Navigate to the URL `https://myapp.com/login`. | Uses a specific, verifiable URL. |
| Try to log in. | Enter "testuser@example.com" into the Username field. | Uses specific input data and target field. |
| Check the homepage. | Verify the user is redirected to the `/dashboard` page. | Verifies a specific endpoint and state change. |

## Test Case Triage and Prioritization

**Triage** is the process of reviewing, ranking, and prioritizing test cases, especially before a release or major testing cycle. This is critical because **Exhaustive Testing is Impossible** (as discussed in Episode 1).

### Key Prioritization Criteria:

* **P1 (Critical):** Tests covering core business workflows (e.g., Payment, Login, Data Saving). If these fail, the product is unusable.
* **P2 (High):** Tests covering major features and common user journeys. Failure impacts a large number of users.
* **P3 (Medium):** Tests covering minor features, edge cases, or less common functionality.
* **P4 (Low):** Tests covering UI aesthetics or documentation accuracy.

## References

* ISTQB (International Software Testing Qualifications Board). (2018). *ISTQB Certified Tester Foundation Level Syllabus*. ISTQB. (Refer to the section on Test Design Techniques and Test Management).
* Whittaker, J. A. (2012). *Exploratory Software Testing: Tips, Tricks, Tours, and Techniques to Guide Test Design*. Addison-Wesley. (While focused on exploration, it emphasizes the clarity needed for documentation).

## 💡 Discussion Question

When reviewing an existing test case, which component (Preconditions, Steps, or Expected Result) do you think is most often missing or poorly defined, and why?
