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



 ## ii. Snapshots
![Pizza Sales Performance Analysis](https://github.com/Morsshed/2.-Power-BI-Sales-Performance-Analysis/blob/main/Pizza%20Sales%20Performance%20Analysis.jpeg?raw=true)


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
 
  #### Overall Performance

       ✓ Total revenue reached $815,306, driven by consistent customer demand.

       ✓ 21,350 orders were recorded, reflecting strong customer activity.

       ✓ A total of 49,574 pizzas were sold.

       ✓ Average order value = $38.19, showing purchases often include multiple items.

       ✓ Average pizzas per order = 2.32, indicating bundling behavior.

  #### Daily & Monthly Trends

       ✓ Fridays and Saturdays generate the highest orders (weekend peaks).

       ✓ Tuesdays and Wednesdays are the slowest sales days.

       ✓ July records the highest monthly orders.

       ✓ October shows the lowest activity.

  #### Category Insights

       ✓ Classic pizzas lead in both revenue and order volume.

       ✓ Supreme pizzas follow closely, showing strong customer preference.

       ✓ Chicken pizzas have the lowest order volume among all categories.

       ✓ Classic category contributes 26.72% of category sales—the largest share.

       ✓ Demand is concentrated mainly in Classic and Supreme, with Veggie and Chicken categories trailing.

  #### Pizza Size Insights

       ✓ Large pizzas are the most purchased size.

       ✓ Medium pizzas also perform well.

       ✓ X-Large pizzas attract a moderate share.

       ✓ XX-Large pizzas have the least demand.

  #### Best & Worst Sellers

       ✓ Thai Chicken Pizza generates the highest revenue among individual pizzas.

       ✓ Thai Barbeque Carre Pizza has the lowest revenue.

       ✓ Classic Deluxe Pizza sells the highest quantity.

       ✓ Mediterranean Pizza records the lowest quantity sold.

       ✓ Classic Deluxe Pizza also leads in total orders.

       ✓ Specialty pizzas like Green, Spinach, and Mediterranean consistently appear in the bottom lists.

  #### Category Breakdown

       ✓ Top-revenue pizzas are dominated by Chicken and Barbecue varieties.

       ✓ Bottom-quantity pizzas include niche flavors with limited customer adoption.

## 📈 Recommendations
       1. Strengthen Midweek Promotions. They can introduce targeted offers on Tuesdays and Wednesdays to lift low-performing days (discounts, bundles, loyalty boosts).

       2. Expand Top-Performing Categories. It is recommended to develop new variations of Classic and Supreme pizzas, as these generate the highest revenue and demand.

       3. Reevaluate Low-Demand Items. They should reformulate, rebrand, or remove consistently low-performing pizzas such as Mediterranean, Green, and Spinach variants.

       4. Promote Large and Medium Size Combos. Since these sizes dominate sales, introduce value deals like family combos or size-based promotions.

       5. Apply Seasonal Strategies. For Example, use targeted campaigns such as i) Summer deals to reinforce July spikes ii) Fall specials to improve October performance.

       6. Highlight Best Sellers. Feature top items (Classic Deluxe, Thai Chicken Pizza) prominently in menus, apps, and ordering platforms.

       7. Align Inventory With Demand. It is better to increase stock for high-demand ingredients (Classic & Supreme), while reducing overstock of low-selling specialty ingredients.
   
 ## v. Data Source
 
 [Pizza Sales Dataset (Kaggle)](https://www.kaggle.com/datasets/shilongzhuang/pizza-sales)

# A - Analysis Techniques:
## A1 -🍕 Data Preparation

### Understanding the Dataset Structure


### Cleaning & Standardization


### Feature Engineering for Analysis


# B - DAX (Data Analysis Expression)
   ### KPI Measures
                    Average Order value = sum(pizza_sales[total_price])/DISTINCTCOUNT(pizza_sales[order_id]) 
                    Average Pizzas Per Order = sum(pizza_sales[quantity])/DISTINCTCOUNT(pizza_sales[order_id])
                    Total Orders = DISTINCTCOUNT(pizza_sales[order_id])
                    Total Pizzas Sold = sum(pizza_sales[quantity])
                    Total Revenue = sum(pizza_sales[total_price])
   ### Calculated Columns
                    Month = left(pizza_sales[Month Name],3)
                    Order Day = left(pizza_sales[Day Name],3)

 # C - Analyses and Interactivities

 ## Daily and Monthly Trend Analysis

![Pizza Sales Performance Dashboard](https://github.com/Morsshed/2.-Power-BI-Sales-Performance-Analysis/blob/main/Pizza%20Sales%20Performance%20Analysis%201.png?raw=true)

 ## Performance Analysis

 ![Pizza Sales Performance Dashboard 2](https://github.com/Morsshed/2.-Power-BI-Sales-Performance-Analysis/blob/main/Pizza%20Sales%20Performance%20Analysis%202.png?raw=true)
