🏥 Healthcare Data Analytics using SQL
📌 Project Overview

This project focuses on analyzing healthcare patient records using PostgreSQL to derive meaningful insights related to patient admissions, discharges, hospital stay duration, demographics, and treatment outcomes.

The dataset contains patient hospitalization details, medical conditions, admission information, and discharge records. Data cleaning, duplicate removal, and analytical queries were performed to answer key healthcare business questions.

🎯 Objectives
Clean and preprocess healthcare data
Remove duplicate patient records
Create reusable SQL views
Analyze patient discharge trends
Measure hospital performance metrics
Understand demographic distributions
Generate actionable healthcare insights
🛠️ Tools & Technologies
PostgreSQL
SQL
Window Functions
Common Table Expressions (CTEs)
Views
Aggregate Functions
Date Functions

📂 Dataset Features

The dataset includes:

Patient ID (MRD Number)
Admission Date
Discharge Date
Age
Gender
Admission Type
Length of Stay
ICU Stay Duration
Treatment Outcome
Smoking & Alcohol History
Diabetes, Hypertension, CAD, CKD Indicators
Laboratory Parameters
Cardiac Conditions
Clinical Diagnoses

🧹 Data Cleaning Process
Duplicate Removal

A view was created using:

CTEs
ROW_NUMBER() Window Function

Duplicate records were identified based on:

MRD Number
Date of Admission
Date of Discharge

Only unique records were retained for analysis.

ROW_NUMBER() OVER(
PARTITION BY "MRD No.","D.O.A","D.O.D"
ORDER BY "MRD No."
)

📊 Business Questions Solved
Hospital Performance Metrics
Total Discharges
Average Daily Discharge Rate
Average Length of Stay
Demographic Analysis
Discharges by Age Group
Pediatric
Adult
Senior Citizen
Discharges by Gender
Time-Based Analysis
Distribution of Discharges by Day of Week

📈 Key Insights Generated

✔ Hospital discharge performance

✔ Patient stay duration trends

✔ Age-group based discharge patterns

✔ Gender-wise patient distribution

✔ Peak discharge days

✔ Data quality improvements through duplicate elimination

SQL Concepts Demonstrated
CTE (WITH Clause)
Views
Window Functions
ROW_NUMBER()
CASE Statements
Aggregate Functions
Date Formatting
Data Cleaning Techniques
Business KPI Calculations
Project Structure
Healthcare-Analytics/
│
├── Healthcare_analysis.sql
├── README.md
│
└── Insights
    ├── Data Cleaning
    ├── Hospital KPIs
    └── Patient Demographics
Learning Outcomes

Through this project, I gained practical experience in:

Healthcare data analysis
SQL-based data cleaning
KPI development
Business-oriented reporting
PostgreSQL query optimization
Real-world analytical problem solving

👨‍💻 Author

Karthik Thakkalapelly

Aspiring Data Analyst skilled in SQL, Power BI, Excel, Python, and Data Visualization.
