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
![WhatsApp Image 2025-11-18 at 7 26 47 PM](https://github.com/user-attachments/assets/4a569368-d0ad-4163-93c3-a2afd5011925)



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
Task 2 Mapping 
![WhatsApp Image 2025-11-18 at 7 25 17 PM](https://github.com/user-attachments/assets/6d60b5cc-559c-4998-be17-26b8d8ba3414)
Master Workflow:
![WhatsApp Image 2025-11-18 at 7 28 38 PM](https://github.com/user-attachments/assets/48f1b8d5-0e36-4616-9b99-8225e890523a)
Monitor 
![WhatsApp Image 2025-11-18 at 7 28 07 PM](https://github.com/user-attachments/assets/2158b0ef-d577-4eb0-a2fc-b1cd484b4b2e)

Summary result:
![WhatsApp Image 2025-11-18 at 7 34 53 PM](https://github.com/user-attachments/assets/cb75acc2-4a54-4b4f-bc8d-83123a67ba35)

🛠 Technologies Used

Informatica PowerCenter (Mappings, Sessions, Workflows)

Oracle SQL

ETL best practices (Layering, transformations, validation)
