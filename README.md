# Expense, Attendance, Grading & Billing Management System

## 1. Project Overview

The Expense, Attendance, Grading & Billing Management System is a menu-driven Python console application developed to automate four common management activities.

The system provides separate modules for expense tracking, attendance calculation, student grading and customer billing. It also generates formatted reports for each module.

## 2. Objectives

- Replace manual calculations with automated calculations.
- Reduce errors through input validation.
- Generate clear and readable reports.
- Provide a simple menu-driven interface.
- Handle invalid input without crashing the application.

## 3. Technologies Used

- **Programming Language:** Python
- **IDE:** PyCharm
- **Interface:** Console-based
- **Storage:** In-memory Python lists and dictionaries
- **Libraries:** Python standard library only

## 4. Project Structure

```text
Expense_and_Attendance_Management/
│
├── main.py
├── validation.py
├── expenses.py
├── attendance.py
├── grading.py
├── billing.py
├── reports.py
├── README.md
└── test_cases.md
```

## 5. Installation and Setup

1. Install Python 3 on your computer.
2. Install and open PyCharm.
3. Create or open the project folder.
4. Place all the Python module files in the same folder.
5. Ensure that the filenames match the project structure.
6. No external Python packages are required.

## 6. How to Run the Application

1. Open the project in PyCharm.
2. Open `main.py`.
3. Right-click inside the editor.
4. Select **Run 'main'**.

Alternatively, open a terminal in the project folder and execute:

```bash
python main.py
```

## 7. Main Menu

The application provides six options:

1. Expense Management
2. Attendance Management
3. Grading System
4. Billing System
5. View Reports
6. Exit

## 8. Features

### A. Expense Management

- Add expenses with description, category and amount.
- Select from Food, Travel, Utilities, Stationery and Other.
- View all recorded expenses.
- Calculate grand total and category-wise totals.
- Identify the highest and lowest expenses.

### B. Attendance Management

- Enter total working days.
- Record a person's name, ID and days present.
- Calculate attendance percentage.
- Assign Eligible, Warning or Shortage status.
- Generate an attendance summary.

### C. Grading System

- Enter marks for a configurable number of subjects.
- Calculate total, average and percentage.
- Assign grades from A+ to F.
- Apply the subject-level failure rule.
- Generate individual report cards and class summaries.

### D. Billing System

- Enter customer and item details.
- Add multiple items to a bill.
- Calculate line totals and subtotal.
- Apply discount slabs of 0%, 5%, 10% or 15%.
- Calculate 18% tax after discount.
- Generate a formatted invoice.

### E. Reports

- Generate expense reports.
- Generate attendance reports.
- Generate grading reports.
- Generate billing reports.
- Export reports to text files.

## 9. Input Validation and Error Handling

The system uses reusable validation functions to check user inputs.

Examples include:

- Names must contain 2–40 alphabetic characters and spaces.
- Expense amounts must be positive and allow up to two decimal places.
- Working days must be positive integers.
- Attendance days must be within the valid range.
- Marks must be between 0 and 100.
- Unit prices must be greater than zero.
- Quantities must be whole numbers of at least 1.

Invalid inputs display helpful messages and prompt the user again.

## 10. Data Storage

The application stores records using Python lists and dictionaries while the program is running.

Data is stored in memory and is not automatically retained after the application exits. Reports can optionally be exported as `.txt` files.

## 11. How to Exit

Select option 6 from the main menu to close the application safely.

The application also handles a keyboard interruption (Ctrl+C) with a graceful exit message.

## 12. Conclusion

This project demonstrates the practical use of Python fundamentals, including variables, data types, operators, conditional statements, loops, functions, lists, dictionaries, tuples, exception handling and formatted strings.

It provides a simple and reusable solution for expense tracking, attendance management, student grading, billing and report generation.
