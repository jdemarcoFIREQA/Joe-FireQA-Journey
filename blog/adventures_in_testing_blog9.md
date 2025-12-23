# Blog 9: Smoke Tests & Regression: Protecting the Ship From Sinking

## Introduction

Software changes constantly. How do we ensure that a new feature or bug fix hasn't broken existing functionality? The answer lies in two critical test types: **Smoke Testing** (a quick health check) and **Regression Testing** (deep verification).

## Smoke Testing: The Quick Health Check

* **Analogy:** A check to see if the server is "smoking" (i.e., immediately broken) after a new build is deployed to the test environment.
* **Definition:** A quick, minimal set of tests that confirms whether the build is stable enough to proceed with further, more comprehensive testing.
* **Key Characteristics:**
    * **Focus:** Core functionality only (e.g., Can the user log in? Can they navigate to the main screen? Can they save data?).
    * **Duration:** Very short (5-15 minutes).
    * **Outcome:** Binary—either the build passes the smoke test and is accepted, or it fails and is rejected immediately.
* **Who Executes:** Often performed first by an automated suite (the automated acceptance test), or a designated tester immediately after a new build.

## Regression Testing: Deep Verification

* **Definition:** Testing to confirm that recent code changes (fixes, additions, or modifications) have not adversely affected existing system functionality.
* **When It Happens:** Before every major release, and ideally, continuously throughout the development process.
* **Scope:** Much broader than a smoke test, covering all critical and high-risk functionality.

### Strategies for Selecting Regression Tests:

1.  **Risk-Based Selection:** Prioritize tests covering high-risk areas (complex code, frequently modified modules, critical business workflows).
2.  **Test Case Traceability:** Select tests that cover requirements directly related to the newly modified code area.
3.  **Automated Suite:** The bulk of regression is usually handled by a comprehensive, automated test suite because manual execution is too time-consuming.

## Re-Testing (Confirmation Testing)

Do not confuse Regression Testing with **Re-Testing** (or Confirmation Testing).

* **Re-Testing:** Executing a specific test case that previously failed to verify that the defect has been successfully fixed by the developer. (It confirms the fix works).
* **Regression Testing:** Executing a wider set of tests to ensure the *fix* itself didn't break anything *else*.

## References

* Pressman, R. S. (2014). *Software Engineering: A Practitioner's Approach* (8th ed.). McGraw-Hill Education. (Discusses validation and regression as key testing types).
* Gerrard, P. (2013). *The Tester's Pocketbook*. Putteridge Books. (Practical distinction between the test types).

## Discussion Question

A developer deploys a fix for a severe bug in the checkout process. As a tester, what is the single most important task you must do: Re-Test the original bug, or run a Regression Test on the rest of the shopping site?
