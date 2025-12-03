# Power-BI-HR-Attrition-Analysis
Analyze and visualize factors influencing HR attrition
 
[Interactive HR Attrition Dashboard (Power BI)](https://app.powerbi.com/view?r=eyJrIjoiZmU2N2FhNWMtODljZC00OTQzLWI4MzUtZDg2MWIyYWZhNjc1IiwidCI6IjFhOTM4M2ZmLTVlMDEtNDkzYy04MTJmLTg0ODAzZTliMGI3YiJ9)


 ###  Domain: Human Resources (HR)

# Analysis Details
 ## i. HR Case
 
##### 🚩 Problem Statement:

The company is experiencing inconsistent attrition trends across departments, age groups, tenure levels, and education categories, raising concerns about employee engagement, workforce stability, and long-term HR planning effectiveness.

##### Key Issues:

► What factors are driving the high attrition rate among younger employees?

► Why are specific departments consistently experiencing higher turnover than others?

► What causes newly hired employees (0–2 years of tenure) to leave at a significantly higher rate than long-tenured staff?

► How do attrition patterns differ across education levels, and which groups are most at risk of leaving?

► What role does job satisfaction play in voluntary exits, and which roles or levels show the lowest engagement?

► How is the loss of skilled employees affecting the company’s productivity, operational stability, and replacement costs?

 ## ii. Snapshot
 
![HR Attrition Analysis](https://github.com/Morsshed/Power-BI-HR-Attrition-Analysis/blob/main/HR%20Attrition%20Analysis.png?raw=true)

 ## iii. Dashboard Features

                             Dynamic Features:
                                              1. Slicers : Doctorate/Associates/Bachelor/Master/High School Degree
                                              2. Cross Filter : Slicers to Visuals
                                              3. Hover : Visual level hovers                
                             Analytical Features:
                                              1. KPI Cards : Total Employee, Total Attrition, Attrition Rate, Total Active Employee, Average Age
                                              2. Column Chart : Total Employee by Age Group
                                              3. Matrix : Job Satisfaction Rating
                                              4. Funnel Chart : Total Pizzas Sold by Pizza Category
                                              7. Pie Charts : Total attrition departments, attrition rate by gender for different age groups
                                              8. Bar Charts : Education Field Wise Attrition
                                              
 ## iv. 🔍 Insights and Recommendations
 
### Overall Workforce Metrics

 ● Total employees = 1470, of which 237 left → Attrition Rate: 16.12%.

 ● Active employees = 1233, indicating a moderate turnover level.

 ● Average employee age is 37, meaning a mid-career workforce.

### Department-wise Insights

 ● R&D and Sales show the highest attrition (largest slices in the pie chart).

 ● HR has the smallest attrition share, indicating higher job stability.

### Age Group Trends

 ● Age group 25–34 has the highest employee count.

 ● Workers aged 35–44 also form a strong portion of the workforce.

 ● Attrition is highest among under 25 and 25–34 age groups.

### Gender Trends

 ● In almost every age group, male attrition slightly exceeds female attrition.

 ● Under 25: Female attrition proportionally higher than male.

 ● Above 55: Very low attrition for both genders.

### Education-wise

 ● Attrition is highest among employees with Bachelor’s and Master’s degrees (largest bars).

 ● High school and technical education groups show low attrition volume.

### Job Satisfaction

 ● Some roles (e.g., Sales Representative, Laboratory Technicians) have many low satisfaction ratings (1–2).

 ● Higher-level managerial roles show relatively better satisfaction.

## 📈 Recommendations

 ✓ Target retention programs for 25–34 age group, where most attrition occurs.

 ✓ Improve satisfaction for Sales & R&D roles, as they show the biggest attrition.

 ✓ Launch career-growth and skill-development programs for bachelor/associate degree groups.

 ✓ Conduct focused exit-interviews to understand dissatisfaction among low-satisfaction roles (lab techs, sales reps).

 ✓ Introduce gender-inclusive engagement strategies, addressing slightly higher male attrition.
   
 ## v. Data Source
 
 [IBM HR Analytics Employee Attrition & Performance Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)


# A - Analysis Techniques:
## A1 - Data Preparation

### Data Collection & Inspection

The HR dataset was collected from [source] and contains employee demographics, job roles, performance metrics, and attrition information. Initial inspection included checking the number of rows and columns, data types, and summary statistics to identify anomalies or inconsistencies. Duplicate entries and obvious errors were removed, and categorical columns were standardized to ensure consistency.

### Data Cleaning & Feature Engineering

Missing values were addressed using appropriate strategies, such as median imputation for numerical fields and mode or “Unknown” labels for categorical fields. Outliers were detected via boxplots and Z-score methods and were either capped or removed to prevent skewed analysis. New features were created to enhance insights, including age groups, experience levels, and work-life balance scores. Categorical variables were encoded for analysis and modeling, with one-hot encoding for nominal data and label encoding for ordinal data.

### Data Transformation & Final Dataset

Numerical features were normalized or standardized to improve model performance and ensure consistency across visualizations. Units and date formats were unified for clarity in dashboards. The cleaned dataset was split into features and target variable (Attrition) and saved as HR_Attrition_Cleaned.csv for use in dashboard visualizations and predictive modeling. A data dictionary was also prepared to describe each column and its role in analysis.

# B - DAX (Data Analysis Expression)
   ### KPI Measures
                    Total Attrition = SUM(HR[Attrition number]) 
                    Average Age = sum(HR[Age])/sum(HR[Employee Count])
                    Attrition Rate = sum(HR[Attrition number])/sum(HR[Employee Count])
                    Active Employee = SUM(HR[Employee Count])-sum(HR[Attrition number])
      
 # C - Analyses and Interactivities


 ## Detailed Insights

 ### 1️⃣ Doctoral Degree 
  
![Doctoral Attrition Analysis](https://github.com/Morsshed/Power-BI-HR-Attrition-Analysis/blob/main/Doctoral%20Attrition.png?raw=true)  

 ● Very small workforce: 17 employees, 1 attrition → 5.88% attrition rate (lowest among all).

 ● Average age = 38, slightly older than overall workforce.

 ● HR shows 0 attrition; distribution well balanced.

 ● Most employees fall between 35–44 age group.

 ● Gender ratio roughly equal.

 ● Attrition almost negligible across all age groups.

 ● Job satisfaction scores are mostly 3–4, showing stable engagement.

 ● No major concentration by department → doctoral roles dispersed.

 ● Education field segments show near-zero attrition.

 ● Doctoral employees appear highly stable and least likely to leave.

### 2️⃣ Associate Degree 
 
![Associate Degree Attrition Analysis](https://github.com/Morsshed/Power-BI-HR-Attrition-Analysis/blob/main/Associate%20Attrition.png?raw=true)

 ● Workforce: 116 employees, 18 attrition → 15.52% attrition rate.

 ● Average age: 36, slightly younger group.

 ● Attrition highest in Sales and R&D sectors.

 ● Most employees aged 25–34.

 ● Attrition slightly higher among males in young age groups.

 ● Under-25 group shows noticeable attrition ratio.

 ● Job satisfaction patterns show more rating 2 and fewer high ratings.

 ● Associate-degree workforce seems entry-level to mid-career.

 ● Education field values indicate more technical-field employees.

 ● Engagement weaker than Master/Doctoral segments.

### 3️⃣ Bachelor’s Degree 

![Bachelor’s Degree Attrition](https://github.com/Morsshed/Power-BI-HR-Attrition-Analysis/blob/main/Bachelor%20Attrition.png?raw=true)

● Largest group: 233 employees, 37 attrition → 15.88% attrition rate.

● Average age = 37.

● This group drives the highest total attrition count after All-Employees view.

● High attrition in R&D and Sales, similar to global pattern.

● Age group 25–34 dominates employment count.

● Under-25 attrition relatively high.

● Male attrition slightly higher in most age segments.

● Job satisfaction varies widely → strong 2–3 ratings distribution.

● Bachelor’s degree shows the largest workforce mobility, meaning more job-switch behavior.

● This group mirrors the overall HR dataset pattern.

### 4️⃣ Master’s Degree 

![Master’s Degree Attrition](https://github.com/Morsshed/Power-BI-HR-Attrition-Analysis/blob/main/Master%20Attrition.png?raw=true)

● Workforce: 173 employees, 25 attrition → 14.45% attrition rate.

● Average age = 39, older and more experienced group.

● R&D and Sales again show the most attrition.

● Most employees in 25–34 and 35–44 age groups.

● Gender distribution balanced; slightly higher male attrition.

● Under-25 nearly zero attrition.

● Job satisfaction slightly better compared to bachelor-level employees.

● Attrition at mid-career (35–44) is noticeable.

● Master’s-level workers appear more stable than bachelor’s holders.

● Education field distribution suggests professional/technical backgrounds.

### 5️⃣ High School Degree

![High School Attrition](https://github.com/Morsshed/Power-BI-HR-Attrition-Analysis/blob/main/High%20School%20Attrition.png?raw=true)

● Small workforce: 67 employees, 8 attrition → 11.94% attrition rate.

● Average age = 34, youngest group overall.

● Department attrition concentrated mainly in Sales.

● Under-25 group very small but shows some attrition.

● Lower overall attrition compared to bachelor/associate degree groups.

● Workforce mostly entry-level operational roles.

● Age group 25–34 has majority of employees.

● Gender attrition difference minimal.

● Job satisfaction ratings stable (many 3–4s).

● High-school group shows better retention than Associate/Bachelor groups.

 # Conclusion

Overall recommendations for Doctoral, Associate, Bachelor, Master, High School graduated employees

✓ Doctoral group needs minimal intervention — maintain current stability through recognition and research-support programs.

✓ Improve job satisfaction for Associate and Bachelor groups by enhancing workload balance and growth opportunities.

✓ Master’s group would benefit from leadership training to reduce mid-career attrition.

✓ High-school workforce should receive structured skill-upgrading programs to improve long-term retention and role mobility.

