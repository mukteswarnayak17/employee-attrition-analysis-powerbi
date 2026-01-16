# Employee Attrition Analysis Dashboard (Power BI)

## 📊 Project Overview
This project is an end-to-end data visualization solution created in **Power BI** to analyze employee turnover. By examining a dataset of 1,470 employees, the dashboard identifies the core reasons behind attrition, such as low salary satisfaction, specific age demographics, and high-pressure job roles. These insights allow HR teams to make data-driven decisions to improve employee retention.

---

## 🛠️ Tools & Technologies
- **Power BI Desktop**: Used for the entire project (ETL, Modeling, and Visualization).
- **Power Query**: Used for data cleaning and creating conditional columns.
- **DAX (Data Analysis Expressions)**: Used to calculate complex KPIs like Attrition Rate and Average Age.
- **Data Source**: IBM HR Analytics (CSV format).

---

## 📁 Project Steps (Completed in Power BI)

### 1. Data Connection & Extraction
- **Dataset Source**: [IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Method**: Imported the raw CSV file directly into Power BI Desktop.

### 2. Data Transformation (Power Query)
- **Data Cleaning**: Handled missing values and removed irrelevant columns (`EmployeeCount`, `StandardHours`, etc.).
- **Salary Slabs**: Created a conditional column to group monthly income into categories (e.g., Upto 5k, 5k-10k, 10k-15k, 15k+).
- **Age Grouping**: Created age bins (18-25, 26-35, 36-45, 46-55, 55+) to identify which age groups are most likely to leave.

### 3. Data Modeling & DAX Measures
Developed several measures to provide deep insights:
- **Total Employees**: `COUNT(HR_Data[EmployeeID])`
- **Attrition Count**: `CALCULATE(COUNT(HR_Data[Attrition]), HR_Data[Attrition] = "Yes")`
- **Attrition Rate**: `[Attrition Count] / [Total Employees]`
- **Average Tenure**: Calculated average years spent at the company.

### 4. Interactive Visualization
Created a professional dashboard layout including:
- **KPI Cards**: Displaying Total Employees, Attrition Count, and Attrition Rate.
- **Donut Charts**: Showing attrition breakdown by **Education Field** and **Gender**.
- **Bar Charts**: Comparing attrition across different **Job Roles** and **Salary Slabs**.
- **Slicers**: Added filters for **Department** to allow for dynamic, departmental-level analysis.

---

## 📈 Results & Insights
- **Salary Impact**: There is a clear trend showing that employees in the **lowest salary slab (Upto 5k)** have the highest attrition rate.
- **Job Role Risks**: **Laboratory Technicians** and **Sales Executives** are the roles with the highest turnover volume.
- **Critical Age Group**: Employees aged **26-35** represent the highest attrition count, indicating a need for better growth opportunities in early-to-mid careers.
- **Education Factor**: Employees with a background in **Life Sciences** and **Medical** fields contribute to the majority of the turnover.

---

## 📋 Requirements
- **Power BI Desktop** (Free download from the Microsoft Store).
- The dataset file: `WA_Fn-UseC_-HR-Employee-Attrition.csv`.

---

## 🧭 Getting Started
1. **Clone the Repo**:
   ```bash
   git clone <your-repository-link>

## 📜 License
**This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments
- **Data Source: IBM HR Analytics via Kaggle.

- **Inspiration: Real-world HR case studies focused on workforce optimization and retention.
