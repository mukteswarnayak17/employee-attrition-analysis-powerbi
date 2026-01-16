Employee Attrition Analysis: Power BI Dashboard Project
📊 Project Overview
This project presents a comprehensive Human Resources (HR) Analytics Dashboard developed to understand and mitigate employee turnover. Using a dataset of 1,470 employees, the dashboard identifies critical attrition drivers—such as age, salary slabs, and job roles—enabling HR departments to transition from reactive reporting to data-driven retention strategies.

🛠️ Tools & Technologies
Platform: Microsoft Power BI Desktop.

Data Transformation: Power Query (M Language).

Analytics Engine: DAX (Data Analysis Expressions) for calculated measures and KPIs.

Data Source: IBM HR Analytics Employee Attrition & Performance (CSV/Excel).

📁 Project Steps
1. Data Connection & Extraction
Source: Kaggle - IBM HR Analytics Dataset.

Process: Integrated the raw CSV into Power BI Desktop via the "Get Data" connector.

2. Data Transformation (Power Query)
Cleaning: Removed redundant columns like EmployeeCount, Over18, and StandardHours which contained single unique values.

Feature Engineering:

Created Conditional Columns for "Salary Slabs" (e.g., Upto 5k, 5k-10k, etc.).

Grouped ages into Age Bins (e.g., 18-25, 26-35, 36-45, 46-55, 55+) for demographic grouping.

Data Typing: Ensured correct formatting for numerical values and categorical attributes.

3. Data Modeling & DAX Measures
KPI Development: Created key measures using DAX, including:

Total Employees = COUNT(EmployeeID).

Attrition Count = CALCULATE(COUNT(Attrition), Attrition="Yes").

Attrition Rate = [Attrition Count] / [Total Employees].

Average Salary and Average Age.

4. Interactive Dashboard Design
Visual Elements:

KPI Cards: High-level overview of total headcount and attrition rates.

Donut/Pie Charts: Attrition distribution by Education Field and Gender.

Bar Charts: Attrition count broken down by Job Role and Salary Slab.

Treemaps/Column Charts: Trends across different Age Groups.

Interactivity: Implemented Slicers for Department and Gender to allow dynamic filtering.

📈 Results & Insights
Role Vulnerability: The Laboratory Technician role often exhibits the highest attrition (62 cases in this dataset).

Income Correlation: Employees in the lowest salary slab (Upto 5k) are significantly more likely to leave the organization.

Education Impact: Attrition is notably higher among those with Life Sciences and Medical backgrounds.

Age Factor: The 26-35 age group typically represents the largest segment of voluntary departures.

📋 Requirements
Software: Microsoft Power BI Desktop (Version: Latest).

System: Windows 10/11 with 4GB+ RAM (8GB recommended for smoother rendering).

License: A free Fabric/Power BI license is sufficient for local exploration.

🧭 Getting Started
Download Dataset: Obtain the WA_Fn-UseC_-HR-Employee-Attrition.csv file from Kaggle.

Open Power BI: Launch the .pbix project file.

Data Source Setting: If prompted, update the file path to point to your local CSV location.

Explore: Use the slicers on the left/top to filter the insights by department or demographic.
