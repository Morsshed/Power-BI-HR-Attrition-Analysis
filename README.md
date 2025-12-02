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
                                              1. Slicers : Pizza Category/Name/Size
                                              2. Button : Pizza Sales Part 1&2
                                              3. Nevigators : Pizza Sales Part 1                  
                             Analytical Features:
                                              1. KPI Cards : Total Orders, Total Revenue, Total Orders, Total Pizza Sold, AVG Order Value, AVG Pizzas Per Order
                                              2. Column Chart : Daily Trends of Orders,
                                              3. Line Chart : Monthly Trends of Orders
                                              4. Funnel Chart : Total Pizzas Sold by Pizza Category
                                              7. Pie Charts : % of Sales by Pizza Category, % of Sales by Pizza Size
                                              8. Bar Charts : Top & Bottom 5 Pizzas by Total Revenue/Total Quantity/Total Order
                                              
 ## iv. 🔍 Insights and Recommendations
 

## 📈 Recommendations

   
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


