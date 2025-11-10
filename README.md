# HR_Data_ETL_Informatica_project
Employee ETL Project
🚀 Employee Performance ETL Pipeline (Informatica PowerCenter)

This project demonstrates an ETL pipeline using Informatica PowerCenter that processes HR data to generate employee performance insights.

📌 Project Overview
Task	Description
Task 1 – Employee Detail Load	Join HR tables, apply business rules, and load detailed employee data into TGT_EMPLOYEE_DETAIL
Task 2 – Department Summary	Aggregate from Task 1 output into department-level performance insights
🧠 Business Rules Implemented
Task 1

✔ Join 4 source tables: EMPLOYEES, DEPARTMENTS, JOBS, LOCATIONS
✔ Filter employees hired in last 25 years (300 months)
✔ Exclude departments related to Sales
✔ Calculate:

FULL_NAME

TOTAL_INCOME = Salary + Salary * Commission

YEARS_OF_SERVICE

SALARY_GRADE (HIGH / MEDIUM / LOW)

✔ Sort by Department ID ASC, Salary DESC
✔ Load ~72 records

Task 2

✔ Aggregate by Department
✔ Calculate:

Employee count

AVG salary, AVG total income

MIN/MAX salary

Count of HIGH salary employees
✔ Derive department performance level:

Top (AVG > 12000)

Average (8000–12000)

Low (<8000)

✔ Load 10–12 summarized department records

🛠 Technologies Used

Informatica PowerCenter (Mappings, Sessions, Workflows)

Oracle SQL

ETL best practices (Layering, transformations, validation)
