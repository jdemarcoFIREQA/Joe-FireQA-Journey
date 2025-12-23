#Exercise 6: Accessibility (A11y) Testing
- **Goal:** practice writing test cases that ensure web elements are usable by people relying on assistive technology (like screen readers). These tests often focus on attributes required by WCAG (Web Content Accessibility Guidelines).
- **Feature:** A simple **Submit Button** on a form
- **Focus:** Attributes, keyboard navigation, and clear descriptive text.

|Scenario|Given|When|Then|
|--------|-----|----|----|
|**Keyboard Focus**|The user is navigating the form using the **keyboard (Tab key)**, and the Submit button is visible.|The user presses the **Tab** key until focus reaches the Submit button.|The Submit button receives a **highly visible focus indicator** *(e.g., a thick blue outline)*, and the **screen reader announces** the element as "Submit button."|
|**Missing Accessible Name**|The user is using a **screen reader** (e.g., JAWS or NVDA).|The screen reader encounters the *<button>* element on the form.|The screen reader **announces meaningful text** based on the button's visible label, and the element has a valid aria-label or inner text.|
|**Color Contrast**|The user is viewing the page in **default contrast settings**.|The user views the Submit button's **background color** and its **text** color.|The color contrast ratio between the foreground text and the background color of the button meets the **WCAG 2.1 AA standard (minimum 4.5:1)**.|
