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


| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Status |
|--------------|---------|-------|----------------|---------------|--------|
| TC01 | Generate a single random date | Click "Generate Random Date" | A valid random date should be generated | A valid random date was generated | Pass |
| TC02 | Generate multiple random dates | Enter number >1 in "Number of Dates" | Correct number of random dates generated | Correct number of dates generated | Pass |
| TC03 | Validate date range | Enter Start Date and End Date | Generated date falls within range | All generated dates were within range | Pass |
| TC04 | Repeated generation | Click Generate multiple times rapidly | System continues generating valid dates | Successfully generated multiple dates | Pass |
| TC05 | Input start date later than end date | Enter Start Date > End Date | System shows error message | No validation; tool generated random date | Fail |
| TC06 | Empty date input | Leave Start/End Date blank | Should use default date range or show message | Default range used | Pass |
| TC07 | Invalid date format | Enter an invalid date format | System should show validation message | Some invalid formats accepted | Fail |
| TC08 | Generate large number of dates | Enter 100+ in "Number of Dates" | System handles request without crash | Successfully generated 100 dates | Pass |
| TC09 | Date format selection | Change output format (MM/DD/YYYY, YYYY-MM-DD) | Generated date matches selected format | Output format correctly displayed | Pass |
| TC10 | UI usability | Verify layout, buttons, and readability | Buttons visible, layout clear, result readable | UI is clean and easy to use | Pass |
| TC11 | Mobile responsiveness | Open on mobile or small screen | Layout adjusts correctly, dates readable | Works well on mobile | Pass |
| TC12 | Copy generated date | Copy button (if exists) | Date copied to clipboard | Not available in current version | N/A (suggestion) |
| TC13 | Rapid random date generation | Click generate 50+ times quickly | System should not freeze | Successfully generated all dates | Pass |

## 6. Usability Observations

The tool is simple and easy to use. The layout is clean and the generate button is clearly visible. The results appear quickly after clicking generate.

Some improvements that could enhance usability include:

- Better validation messages for incorrect inputs
- Option to copy generated dates
- Ability to export generated dates
