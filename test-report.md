# Random Date Generator – Test Report

Application: Random Date Generator  
URL Tested: https://codebeautify.org/generate-random-date  
Tester: Priyanka Raghav  
Testing Type: Manual Testing  
Date: 9 March 2026

## 1. Testing Objective

The goal of this testing exercise was to evaluate the functionality and usability of the Random Date Generator tool. The testing focused on verifying whether the application correctly generates random dates based on user inputs and whether it handles edge cases and invalid inputs properly.

## 2. Scope of Testing

The testing scope was limited to the Random Date Generator feature only.

### In Scope
- Generating random dates
- Selecting date ranges
- Generating multiple dates
- Verifying date format
- Basic input validation

### Out of Scope
- Other tools available on the website
- Backend implementation
- Performance under heavy traffic

## 3. Test Environment

Browser: Google Chrome  
Operating System: macOS  
Device: MacBook

## 4. Features Tested

- Generate random date functionality
- Date generation within a selected range
- Output formatting
- Handling of invalid inputs
- Repeated date generation

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
| TC13 | Copy generated date | Copy button | Able to copy | Not available | N/A | IMP-001 |
| TC14 | Start Date = End Date | Enter same date | Only one date | One date generated | Pass | IMP-002 |

## 6. Usability Observations

The tool is simple and easy to use. The layout is clean and the generate button is clearly visible. The results appear quickly after clicking generate.

Some improvements that could enhance usability include:

- Better validation messages for incorrect inputs
- Option to copy generated dates
- Ability to export generated dates
