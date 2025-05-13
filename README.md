🔍 Overview of PAYROLL.ahk Script
This AutoHotkey script is designed to calculate the net monthly salary of an employee, including deductions, bonuses, overtime, and wage adjustments. It uses a GUI (Graphical User Interface) to collect user input and then performs calculations based on this data.

📋 Key Functionalities
Input Collection
The GUI allows the user to enter:
Base salary
Insurance contributions (IKA, TEA, etc.)
Advances or deductions
Number of workdays and hours
Overtime hours (categorized by type)
It also takes percentage rates for various contributions and surcharges.
Calculation Logic
The script calculates:
Net salary = Gross - Deductions + Bonuses
Overtime pay for each type using formulas like:
overtimePay := hourlyRate * hours * multiplier

Total deductions are subtracted from the gross pay.
Adjustments like absences or loans are also considered.
Output Display
Results are displayed in a formatted GUI output, showing:
Total earnings
Overtime breakdown
Deductions
Final payable amount
File Saving
The script creates a monthly .txt file storing:
The calculation details
Employee data
Timestamp
The filename includes the current month and year.
Modular Design
Each category of pay (overtime, bonuses, deductions) has its own input section.
Variables are clearly named according to their use (e.g., nightPay, holidayPay, ikaDeduction).

🔧 Technical Details
AutoHotkey Version: v1 (legacy)
GUI Creation: Uses traditional Gui, Add commands
Math: Arithmetic operations are simple and linear; no use of arrays or objects.
No use of functions or classes, so it's procedural and monolithic.
No input validation, so it's prone to user error (e.g., entering text where a number is expected).

⚠️ Limitations / Room for Improvement
Issue	Suggested Fix
Outdated syntax (AHK v1)	Convert to AHK v2
No input validation	Add checks for numeric input
Procedural structure	Modularize with functions
GUI is basic	Add dropdowns, labels, tooltips
No error handling	Use try/catch in AHK v2
No saving to Excel/CSV	Add export option

✅ Summary
The script is a well-structured prototype for a payroll system, tailored for manual input and monthly storage. With proper modernization (to AHK v2 or porting to another platform like Unity for Android), it can be turned into a fully professional app.

