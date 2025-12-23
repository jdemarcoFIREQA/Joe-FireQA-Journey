# Blog 3: Bug Reporting 101: Making Your Bugs Count

## Introduction

A bug report is the primary communication tool between the tester and the developer. A poor report wastes time; a great report leads to a quick fix and a better product. This blog focuses on writing clear, concise, and complete reports that prioritize reproducibility.

## The Anatomy of a Perfect Bug Report

A perfect bug report is a self-contained unit of information that tells a story of failure.

1.  **Title:** Short, descriptive, and actionable. **DO NOT** use emotional language.
    * *Bad:* "The site is broken when I try to pay."
    * *Good:* "Checkout: Application crashes when user applies two discount codes."
2.  **Environment Details:** Where did the bug happen? (e.g., Browser/Version, OS, Device, Test Environment URL).
3.  **Steps to Reproduce:** The precise, numbered steps that consistently lead to the defect. This is the **most crucial** part of the report. (Ideally, fewer than 6 steps).
4.  **Actual Result:** What actually happened when you executed the final step.
5.  **Expected Result:** What should have happened according to the requirements or design.
6.  **Attachments:** Screenshots, screen recordings, or log files. **Visual proof is golden.**

## Severity vs. Priority: Understanding the Difference

These terms determine how urgently and quickly a bug is fixed. They are distinct concepts:

| Attribute | Severity | Priority |
| :--- | :--- | :--- |
| **Definition** | The **impact** of the defect on the system's functionality. | The **order** in which the defect should be fixed relative to others. |
| **Who Determines** | Primarily the **Tester**. | Primarily the **Product Owner/Manager**. |
| **Example** | An aesthetic issue is Low Severity. A complete crash is Critical Severity. | A critical bug found in a feature launching next week is High Priority. |

A high-severity bug might be low priority if it's in a rarely used feature scheduled for deprecation next quarter.

## The Power of Reproducibility

A developer cannot fix a bug they cannot reproduce. Always attempt to reproduce a bug three times before logging it, and try to isolate the minimum necessary steps.

**Checklist for Reproducibility:**

* Did I use fresh test data?
* Can I reproduce it on a different browser/device?
* Did I clear my cache/cookies? (If applicable)
* Are the exact steps listed in the report?

## References

* Kaner, C., Falk, J., & Nguyen, H. Q. (1999). *Testing Computer Software* (2nd ed.). Wiley. (Foundational work emphasizing the importance of detailed bug documentation).
* Myers, G. J., Sandler, C., & Badgett, T. (2011). *The Art of Software Testing* (3rd ed.). Wiley. (Discusses the need for high-quality, actionable reports).

## Discussion Question

You find a bug that only occurs 1 out of 10 times. How would you handle the "Steps to Reproduce" section of your report to ensure the developer takes it seriously?
