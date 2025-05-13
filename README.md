
 PAYROLL.ahk - Payroll Tool
==========================

Version: AutoHotkey v1
Author: Mavroeidis Anastasios (Tasos)

Description:
-------------
PAYROLL.ahk is a script designed to calculate an employee’s net monthly salary.
It uses a simple Graphical User Interface (GUI) for data input and performs:

- Net salary calculation
- Overtime and surcharge pay
- Insurance deductions (IKA, TEA, etc.)
- Adjustments for advances, absences, or loans
- Various types of premium pay (night, Sunday, overtime, etc.)

Main Features:
---------------
1. GUI Input for:
   - Base gross salary
   - Insurance contributions (IKA, TEA)
   - Advances, absences
   - Work and overtime hours
   - Percentage multipliers for overtime types

2. Calculation:
   - Net = Gross - Deductions + Bonuses
   - Overtime pay = hourlyRate * hours * multiplier
   - Each type of premium pay is calculated separately

3. File Saving:
   - Generates a .txt file per month
   - Includes timestamp, employee details, breakdown of payments
   - Filename format: Payroll_2025_05.txt

4. Output Display:
   - Shows total earnings, overtime breakdown, deductions, net pay

Technical Info:
----------------
- Built with AutoHotkey v1
- Uses traditional GUI (Gui, Add commands)
- No input validation (user must enter correct numeric values)
- Fully procedural, no functions or objects
- Saves data in plain text files

Limitations:
-------------
- Outdated AHK v1 syntax
- No error handling or validation
- Basic GUI without dropdowns or tooltips
- No export to Excel or CSV

Planned Improvements:
-----------------------
- Port to AHK v2
- Add input validation and error checks
- Refactor to use functions and modular code
- Enhanced GUI with dropdowns and hints
- Export results to CSV/Excel
- Android version via Unity

Sample Output:
---------------
Employee: George Papadopoulos  
Gross: €1,100  
Overtime:
 - Night (10h): €125  
 - Sunday (6h): €135  
Deductions:
 - IKA: €180  
 - TEA: €50  
Net Pay: €1,130  
Date: 01/05/2025

How to Use:
------------
1. Install AutoHotkey v1 from www.autohotkey.com
2. Double-click PAYROLL.ahk to run it
3. Fill in the fields and click "Calculate"
4. A results file is saved automatically in the same folder

License:
---------
Free to use, modify, and distribute.  
Impersonating the author is forbidden unless you're Tasos himself 😎

Contact:
---------
Mavroeidis Anastasios  
Nea Ionia, Athens, Greece  
Mail: maxiths1984@gmail.com 
