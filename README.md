# HR Analytics - Employee Attrition & Retention Dashboard

## 📌 Project Overview
This end-to-end Power BI project delivers an executive-level HR dashboard designed to track employee turnover (Attrition Rate), isolate high-risk retention segments, and uncover correlations between job satisfaction and employee flight risks. 

## 🛡️ Enterprise Security: Row-Level Security (RLS)
To comply with strict corporate data privacy standards regarding sensitive payroll and HR metrics, this model features **Row-Level Security (RLS)**. 
- Designed and deployed dynamic roles (e.g., `IT_Manager`) that automatically restrict data visibility based on user department.
- A department head viewing this report will only see headcount metrics, satisfaction indexes, and attrition trends for their specific team, leaving other corporate divisions secure and hidden.

## 🛠️ Tech Stack & Skills
- **Data Engineering:** In-model data schema setup with dedicated measure storage (`_Measures`).
- **Advanced DAX Logic:** Conditional segmentation via multi-layered `SWITCH(TRUE(), ...)` to dynamically bin employee seniority.
- **Calculated Measures:** Developed precision KPIs using safe-division handling via `DIVIDE` and context manipulation via `CALCULATE`.
- **Analytical Layers:** Attrition tracking by seniority groups, cross-filtering satisfaction metrics, and data view simulation.

## 📊 Strategic Business Insights
1. **Onboarding Risk Factor:** Discovered a major retention gap in the newly hired segment (**0-2 Years** of seniority), which exhibits a staggering **~71%** attrition rate, signaling a critical need to overhaul the employee onboarding pipeline.
2. **Satisfaction Correlation:** Verified an absolute 100% turnover rate among employees reporting a `JobSatisfaction` level of 1. Conversely, employees with a satisfaction score of 3 or 4 yielded 0% attrition, validating that mid-tier satisfaction levels are highly predictive of employee loyalty.
