# Test Cases – Expense, Attendance, Grading & Billing Management System

## 1. Testing Overview

**Project:** Expense, Attendance, Grading & Billing Management System  
**Testing Type:** Functional Testing, Input Validation Testing and Boundary Testing  
**Total Test Cases:** 20  
**Testing Environment:** Python 3, PyCharm, Windows

### Testing Objectives

- Verify that all six main menu options work correctly.
- Check that valid inputs are accepted.
- Check that invalid inputs are rejected with appropriate messages.
- Verify calculations for expenses, attendance, grading and billing.
- Verify report generation when records are available and when no records exist.
- Check that the application exits safely.

## 2. Test Case Details

| Test ID | Test Scenario | Test Input / Steps | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|
| TC-01 | Open Expense Module | Enter `1` in main menu | Expense Management menu opens | Pending | Pending |
| TC-02 | Invalid menu input (text) | Enter `abc` | Invalid choice message; application continues | Pending | Pending |
| TC-03 | Invalid menu input (number) | Enter `9` | Invalid choice message; application continues | Pending | Pending |
| TC-04 | Add valid expense | Description: Lunch; Category: Food; Amount: 250.50 | Expense is saved successfully | Pending | Pending |
| TC-05 | Invalid expense amount | Enter `abc`, then `-100` | Invalid amounts rejected; user is prompted again | Pending | Pending |
| TC-06 | Expense amount boundary | Enter amount `0.01` | Minimum positive amount is accepted | Pending | Pending |
| TC-07 | Attendance eligibility boundary | Total days: 40; Present: 30 | Attendance = 75%; Status = Eligible | Pending | Pending |
| TC-08 | Attendance warning status | Total days: 40; Present: 29 | Attendance = 72.50%; Status = Warning | Pending | Pending |
| TC-09 | Attendance exceeds working days | Total days: 40; Present: 41 | Input rejected; user is prompted again | Pending | Pending |
| TC-10 | Zero working days | Enter total working days `0` | Input rejected; positive integer required | Pending | Pending |
| TC-11 | Highest grade calculation | Enter marks `90` in all five subjects | Percentage = 90%; Grade = A+; Result = PASS | Pending | Pending |
| TC-12 | Subject-level failure | Enter marks 90, 90, 34, 90, 90 | Final result = FAIL because one subject is below 35 | Pending | Pending |
| TC-13 | Marks above maximum | Enter marks `105` | Input rejected; maximum marks are 100 | Pending | Pending |
| TC-14 | Non-numeric marks | Enter `eighty` | Input rejected; user is prompted again | Pending | Pending |
| TC-15 | Billing without discount | Add one item: Price = 500; Quantity = 1; then type `done` | Subtotal = 500; Tax = 90; Grand Total = 590 | Pending | Pending |
| TC-16 | Billing discount boundary | Add items with subtotal exactly 1000 | Discount rate = 5%; discount amount = 50 | Pending | Pending |
| TC-17 | Invalid billing quantity | Enter quantity `0` | Quantity rejected; minimum quantity is 1 | Pending | Pending |
| TC-18 | Billing without items | Select Create Bill and type `done` immediately | No bill is created; no-items message displayed | Pending | Pending |
| TC-19 | Reports without records | Open Reports before adding any records | Appropriate no-records messages displayed | Pending | Pending |
| TC-20 | Graceful application exit | Press Ctrl+C while application is running | Application displays interruption message and exits safely | Pending | Pending |

## 3. Additional Calculation Verification

### TC-07 – Attendance Calculation

- Total working days: 40
- Days present: 30
- Calculation: (30 / 40) × 100
- Expected attendance: 75.00%
- Expected status: Eligible

### TC-08 – Attendance Calculation

- Total working days: 40
- Days present: 29
- Calculation: (29 / 40) × 100
- Expected attendance: 72.50%
- Expected status: Warning

### TC-15 – Billing Calculation

- Item price: 500
- Quantity: 1
- Subtotal: 500.00
- Discount: 0.00
- Taxable amount: 500.00
- Tax at 18%: 90.00
- Grand Total: 590.00

### TC-16 – Billing Discount Calculation

- Subtotal: 1000.00
- Discount rate: 5%
- Discount amount: 50.00
- Taxable amount: 950.00
- Tax at 18%: 171.00
- Grand Total: 1121.00

## 4. Test Execution Record

Fill this section after executing the test cases.

| Test ID | Actual Result | Status (Pass/Fail) | Remarks / Bug Fixed |
|---|---------------|---|---|
| TC-01 | Pending       | Pending | |
| TC-02 | Pending       | Pending | |
| TC-03 | Pending       | Pending | |
| TC-04 | Pending       | Pending | |
| TC-05 | Pending       | Pending | |
| TC-06 | Pending       | Pending | |
| TC-07 | Pending       | Pending | |
| TC-08 | Pending       | Pending | |
| TC-09 | Pending       | Pending | |
| TC-10 | Pending       | Pending | |
| TC-11 | Pending       | Pending | |
| TC-12 | Pending       | Pending | |
| TC-13 | Pending       | Pending | |
| TC-14 | Pending       | Pending | |
| TC-15 | Pending       | Pending | |
| TC-16 | Pending       | Pending | |
| TC-17 | Pending       | Pending | |
| TC-18 | Pending       | Pending | |
| TC-19 | Pending       | Pending | |
| TC-20 | Pending       | Pending | |

## 5. Testing Conclusion

Testing will be considered complete after all 20 test cases have been executed.

The application should:
- Accept valid inputs.
- Reject invalid and out-of-range inputs.
- Calculate totals, percentages, grades, discounts and taxes correctly.
- Generate readable reports.
- Handle empty records and keyboard interruption safely.

**Final Testing Result:** Pending execution of test cases.