# Bug / Issue Report – Random Date Generator

**Application:** Random Date Generator  
**URL Tested:** https://codebeautify.org/generate-random-date  
**Tester:** Priyanka Raghav  
**Testing Type:** Manual Testing  
**Date:** March 2026  

---

## 1. BUG‑001
**Title:** No validation when Start Date is later than End Date  
**Severity:** Medium  
**Priority:** High  
**Steps to Reproduce:**  
1. Open the Random Date Generator page  
2. Enter a Start Date that is later than the End Date  
3. Click **Generate**  
**Expected Result:**  
System should display an error message: "Start Date must be earlier than End Date"  
**Actual Result:**  
The tool does not prevent the incorrect input and still generates a date.  
**Impact:**  
Can produce invalid or unexpected results for testing purposes  

---

## 2. BUG‑002
**Title:** Invalid date formats accepted  
**Severity:** Low  
**Priority:** Medium  
**Steps to Reproduce:**  
1. Enter Start or End Date in an invalid format (e.g., "2026/31/12")  
2. Click **Generate**  
**Expected Result:**  
System should show a validation message or reject the input  
**Actual Result:**  
Some invalid date formats are accepted  
**Impact:**  
Could confuse users and produce unintended results  

---

## 3. BUG‑003
**Title:** Output format mismatch  
**Severity:** Low  
**Priority:** Medium  
**Steps to Reproduce:**  
1. Select output format `YYYY-MM-DD`  
2. Generate multiple dates  
**Expected Result:**  
All dates should match the selected format  
**Actual Result:**  
Some dates are still displayed as `MM/DD/YYYY`  
**Impact:**  
Confuses users relying on a consistent format  

---

## 4. BUG‑004
**Title:** Large number of dates may crash system  
**Severity:** Medium  
**Priority:** Medium  
**Steps to Reproduce:**  
1. Enter `10,000` in "Number of Dates" field  
2. Click **Generate**  
**Expected Result:**  
System should limit input or show warning  
**Actual Result:**  
Tool tries to generate all dates, causing browser to crash 
**Impact:**  
Can crash browser or degrade performance  

---

## 5. BUG‑005
**Title:** Leap year edge cases not validated  
**Severity:** Medium  
**Priority:** Medium  
**Steps to Reproduce:**  
1. Start Date = 2021-01-01, End Date = 2021-12-31  
2. Generate multiple dates  
**Expected Result:**  
February 29 should not appear  
**Actual Result:**  
Tool sometimes generates February 29 incorrectly  
**Impact:**  
Generates invalid dates  

---

## 6. BUG‑006
**Title:** UI responsiveness issue on small screens  
**Severity:** Low  
**Priority:** Low  
**Steps to Reproduce:**  
1. Open page on mobile or small window  
2. Generate multiple dates  
**Expected Result:**  
Output should be readable and properly formatted  
**Actual Result:**  
Output may overflow or be cut off  
**Impact:**  
Poor usability on mobile devices  

---

## 7. IMP‑001 (Feature Suggestion)
**Title:** Copy-to-Clipboard functionality  
**Severity:** N/A  
**Priority:** Low  
**Description:**  
Currently, users cannot easily copy generated dates since copy image is in wrong place near generate date button
**Suggested Fix:**  
Add a **copy button** next to output for easy copying  

---

## 8. IMP‑002 (UX Suggestion)
**Title:** Start Date = End Date  
**Severity:** N/A  
**Priority:** Low  
**Description:**  
When Start Date = End Date, only one date is generated  
**Suggested Improvement:**  
Show a small note in the UI explaining this to the user
