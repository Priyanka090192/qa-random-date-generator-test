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

| Test Case | Scenario | Expected Result | Status |
|-----------|----------|----------------|--------|
| TC01 | Generate random date | System should generate a valid date | Pass |
| TC02 | Generate multiple dates | System should display multiple dates | Pass |
| TC03 | Validate date range | Generated date should be within selected range | Pass |
| TC04 | Repeated generation | System should continue generating dates without error | Pass |

## 6. Usability Observations

The tool is simple and easy to use. The layout is clean and the generate button is clearly visible. The results appear quickly after clicking generate.

Some improvements that could enhance usability include:

- Better validation messages for incorrect inputs
- Option to copy generated dates
- Ability to export generated dates
