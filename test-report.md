# Random Date Generator – Test Report

**Application:** Random Date Generator  
**URL Tested:** https://codebeautify.org/generate-random-date  
**Tester:** Priyanka Raghav  
**Testing Type:** Manual Testing  
**Date:** 9 March 2026

---

## 1. Testing Objective

The goal of this testing exercise was to evaluate the functionality, usability, and robustness of the Random Date Generator tool. The focus was on verifying correct date generation based on user inputs, handling edge cases, and validating input restrictions.

---

## 2. Scope of Testing

The testing scope was limited to the Random Date Generator feature.

### In Scope
- Generating random dates  
- Selecting date ranges  
- Generating multiple dates  
- Verifying date format  
- Input validation  
- Basic UI usability  

### Out of Scope
- Other tools on the website  
- Backend implementation  
- Performance under high traffic (except large number input test)  

---

## 3. Test Environment

- **Browser:** Google Chrome  
- **Operating System:** macOS  
- **Device:** MacBook  

## 4. Features Tested

- Generate a single random date  
- Generate multiple random dates at once  
- Generate dates within a specific Start Date and End Date range  
- Validate input dates (Start Date <= End Date)  
- Validate date format selection (MM/DD/YYYY, YYYY-MM-DD)  
- Handle empty date inputs using default range  
- Repeated date generation without errors  
- Leap year and boundary date checks (e.g., Feb 29 on non-leap years)  
- UI usability: button visibility, layout clarity, result readability  
- Mobile responsiveness on small screens  
- Handling large number of dates (stress testing)  
- Negative testing with invalid date formats  
- Feature suggestions: copy-to-clipboard functionality, clear UX when Start Date = End Date

## 5. Test Scenarios


| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Status | Bug ID / Notes |
|--------------|---------|-------|----------------|---------------|--------|----------------|
| TC01 | Generate a single random date | Click "Generate Random Date" | Valid random date generated | Valid date generated | Pass | - |
| TC02 | Generate multiple random dates | Enter number >1 | Correct number generated | Correct number generated | Pass | - |
| TC03 | Validate date range | Enter Start/End Date | Dates within range | Dates within range | Pass | - |
| TC04 | Repeated generation | Click generate repeatedly | Dates continue to generate | Successfully generated | Pass | - |
| TC05 | Start Date > End Date | Enter invalid range | Error message | Tool generated date | Fail | BUG-001 |
| TC06 | Empty date input | Leave blank | Use default range | Default range used | Pass | - |
| TC07 | Invalid date format | Enter invalid format | Error message | Some formats accepted | Fail | BUG-002 |
| TC08 | Large number of dates | Enter 10,000 | System handles request | Tool slowed down | Fail | BUG-004 |
| TC09 | Output format selection | Select YYYY-MM-DD | Dates match format | Some mismatch | Fail | BUG-003 |
| TC10 | Leap year check | Non-leap year Feb 29 | No Feb 29 | Feb 29 sometimes generated | Fail | BUG-005 |
| TC11 | UI usability | Layout, buttons | Clear layout | UI clean | Pass | - |
| TC12 | Mobile responsiveness | Small screen | Output readable | Some overflow | Fail | BUG-006 |
| TC13 | Copy generated date | Click copy button | Able to copy generated dates | Copy button works correctly and copies date | Pass | IMP-001 |
| TC14 | Start Date = End Date with multiple count | Enter same Start and End Date and request multiple dates | All generated dates should respect the date range | Same date repeated for all outputs | Pass / Observation | IMP-002 (UX Note) |

## 6. Issue Identified

The following critical issues were identified during testing:

- **BUG‑001:** No validation when Start Date > End Date  
- **BUG‑002:** Some invalid date formats accepted  
- **BUG‑003:** Output format mismatch  
- **BUG‑004:** Large number of dates may slow down system  
- **BUG‑005:** Leap year edge cases not handled  
- **BUG‑006:** Mobile responsiveness issues  

Feature improvements suggested:  
- **IMP‑001:** Copy-to-Clipboard functionality wrong placement  
- **IMP‑002:** UX clarification when Start Date = End Date  

---
## 7. Usability Observations

- The tool is simple, clean, and easy to use.  
- The generate button is clearly visible and accessible.  
- Output appears quickly after clicking generate.  

Suggested improvements:  
- Provide clear validation messages for incorrect inputs.  
- Add copy-to-clipboard functionality for generated dates.  
- Include visual hints or notes when Start Date = End Date.  
- Improve mobile layout for smaller devices.  

---

## 8. Conclusion

The Random Date Generator performs its primary function effectively, generating random dates as expected. Most core features work well, and the tool is easy to use.  

However, input validation for date ranges and formats, mobile responsiveness, and additional usability features could be improved. Addressing these issues would enhance reliability and user experience.  

---
