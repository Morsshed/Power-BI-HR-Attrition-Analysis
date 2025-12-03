# Power-BI-HR-Attrition-Analysis
Analyze and visualize factors influencing HR attrition
 
[Interactive HR Attrition Dashboard (Power BI)](https://app.powerbi.com/view?r=eyJrIjoiZmU2N2FhNWMtODljZC00OTQzLWI4MzUtZDg2MWIyYWZhNjc1IiwidCI6IjFhOTM4M2ZmLTVlMDEtNDkzYy04MTJmLTg0ODAzZTliMGI3YiJ9)


 ### 1. Domain: Human Resources (HR)

# Analysis Details
 ## i. HR Case
 
##### 🚩 Problem Statement:

The pizza business shows strong overall sales, but key performance drivers remain unclear. The company lacks detailed insights into customer behavior, product performance, and demand patterns, making it difficult to optimize operations and maximize revenue.

##### Key Issues:

✔️ Uncertainty about which pizza categories, sizes, and individual items drive the most revenue.

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

 ✓ Total employees = 1470, of which 237 left → Attrition Rate: 16.12%.

 ✓ Active employees = 1233, indicating a moderate turnover level.

 ✓ Average employee age is 37, meaning a mid-career workforce.

### Department-wise Insights

 ✓ R&D and Sales show the highest attrition (largest slices in the pie chart).

 ✓ HR has the smallest attrition share, indicating higher job stability.

### Age Group Trends

 ✓ Age group 25–34 has the highest employee count.

 ✓ Workers aged 35–44 also form a strong portion of the workforce.

 ✓ Attrition is highest among under 25 and 25–34 age groups.

### Gender Trends

 ✓ In almost every age group, male attrition slightly exceeds female attrition.

 ✓ Under 25: Female attrition proportionally higher than male.

 ✓ Above 55: Very low attrition for both genders.

### Education-wise

 ✓ Attrition is highest among employees with Bachelor’s and Master’s degrees (largest bars).

 ✓ High school and technical education groups show low attrition volume.

### Job Satisfaction

 ✓ Some roles (e.g., Sales Representative, Laboratory Technicians) have many low satisfaction ratings (1–2).

 ✓ Higher-level managerial roles show relatively better satisfaction.

## 📈 Recommendations

 ✓ Target retention programs for 25–34 age group, where most attrition occurs.

 ✓ Improve satisfaction for Sales & R&D roles, as they show the biggest attrition.

 ✓ Launch career-growth and skill-development programs for bachelor/associate degree groups.

 ✓ Conduct focused exit-interviews to understand dissatisfaction among low-satisfaction roles (lab techs, sales reps).

 ✓ Introduce gender-inclusive engagement strategies, addressing slightly higher male attrition.
   
 ## v. Data Source
 
 [Pizza Sales Dataset (Kaggle)](https://www.kaggle.com/datasets/shilongzhuang/pizza-sales)

# A - Analysis Techniques:
## A1 -🍕 Data Preparation

# B - DAX (Data Analysis Expression)
   ### KPI Measures
                    Total Attrition = SUM(HR[Attrition number]) 
                    Average Age = sum(HR[Age])/sum(HR[Employee Count])
                    Attrition Rate = sum(HR[Attrition number])/sum(HR[Employee Count])
                    Active Employee = SUM(HR[Employee Count])-sum(HR[Attrition number])
      
 # C - Analyses and Interactivities

![HR Attrition Analysis](https://github.com/Morsshed/Power-BI-HR-Attrition-Analysis/blob/main/HR%20Attrition%20Analysis.png?raw=true)

 ## Detailed Insights

 # Conclusion


