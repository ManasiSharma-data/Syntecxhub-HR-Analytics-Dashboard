# 📊 HR Analytics Dashboard (Power BI)

## 📌 Project Overview
This project focuses on analyzing employee data to understand workforce trends, attrition patterns, and key HR metrics. The dashboard helps in making data-driven HR decisions.

---

## 🎯 Key Features
- Interactive HR Dashboard
- Employee Attrition Analysis
- Department & Job Role Insights
- Salary Distribution Analysis
- Gender-wise Workforce Insights

---

## 📊 KPIs Used
- Total Employees
- Attrition Count
- Attrition Rate
- Average Salary
- Retention Rate

---

## 📈 Visualizations
- Attrition by Department (Bar Chart)
- Attrition by Job Role (Column Chart)
- Salary vs Attrition (Clustered Chart)
- Gender-wise Attrition (Pie Chart)
- Attrition by Age Group (Bar Chart)
- Department-wise Salary Analysis

---

## 🎛️ Filters (Slicers)
- Department
- Gender
- Job Role
- Age Group

---

## 🧮 DAX Measures
```DAX
Total Employees = COUNT(Employee[EmployeeID])

Attrition Count = 
CALCULATE(COUNT(Employee[EmployeeID]), Employee[Attrition] = "Yes")

Attrition Rate = 
DIVIDE([Attrition Count], [Total Employees]) * 100

Avg Salary = AVERAGE(Employee[Salary])

Retention Rate = 100 - [Attrition Rate]
