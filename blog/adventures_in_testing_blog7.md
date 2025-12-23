# Blog 7: Agile Adventures: Testing in Sprints and Scrum

## Introduction

Modern software development overwhelmingly uses Agile methodologies, primarily Scrum. The tester's role changes dramatically in this environment, moving from a final gatekeeper to an integrated team member. This blog explores the life of a tester in a two-week sprint cycle.

## Testing in the Agile Cycle

The core concept is **continuous feedback** and testing.

| Scrum Event | Tester’s Key Involvement |
| :--- | :--- |
| **Sprint Planning** | Help define acceptance criteria for user stories; provide effort estimates for testing tasks. |
| **Daily Stand-up (Scrum)** | Report on progress, current blockers, and readiness of features for testing; highlight potential risks. |
| **Development** | **Shift Left!** Test code incrementally, pair with developers, review unit test coverage, and start writing automated tests *before* the feature is complete. |
| **Feature Complete** | Final exploratory and functional testing; running regression suites. |
| **Sprint Review** | Demo tested features to stakeholders; advocate for quality. |
| **Sprint Retrospective** | Discuss what went well/poorly regarding quality, process, and tools; propose improvements. |

## The Definition of "Done"

The **Definition of Done (DoD)** is a critical checklist that all work must satisfy before a User Story can be considered complete and shippable. The tester is a key guardian of the DoD.

### Sample Tester Items in the DoD:

* All Acceptance Criteria are met.
* All unit tests are passing.
* Required **Exploratory Testing** sessions are completed.
* No **Severity 1 or 2** bugs are open.
* Test cases are documented and updated in the Test Management Tool.

## The "Ready" State

Before a user story can be pulled into a sprint for development, it should meet the **Definition of Ready (DoR)**. The tester helps verify:

* The user story is clearly understood.
* Acceptance Criteria are well-defined and **testable**.
* Dependencies are identified and resolved.

## References

* Schwaber, K., & Sutherland, J. (2020). *The Scrum Guide*. Scrum.org. (The authoritative source for Scrum methodology).
* Crispin, L., & Gregory, J. (2009). *Agile Testing: A Practical Guide for Testers and Agile Teams*. Addison-Wesley. (The seminal book on the tester's role in Agile).

## 💡 Discussion Question

How can a tester best contribute to the **Sprint Planning** meeting beyond just providing time estimates for testing?
