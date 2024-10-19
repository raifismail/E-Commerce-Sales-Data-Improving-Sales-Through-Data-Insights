   ## E-Commerce-Sales-Data-Improving-Sales-Through-Data-Insights

# Project Overview

This e-commerce case study analyzes six months of sales data to identify key business insights and trends. The dataset includes information such as order ID, date, product category, region, quantity sold, unit price, and total sales. The project focuses on visualizing and analyzing sales performance across different product categories, regions, and time periods to derive actionable insights for the business.

# Business Task

The goal of this project was to analyze the sales data of an e-commerce platform to provide actionable insights that can drive business growth. Specifically, we aimed to answer the following key questions:

   - Identifying regional sales performance to target future marketing efforts.

   - Understanding which product categories drive the most revenue to optimize inventory and product promotion strategies.

   - Analyzing monthly sales trends to spot seasonality and plan promotional campaigns more effectively.

   - Examining the sales trends across regions to identify regional growth opportunities and potential sales strategies.
     
# Data cleaning 

 - sql code used for data cleaning and anlysis added in repository you can find it [here]()
Before analyzing the data, I performed the following data cleaning steps to ensure the dataset was ready for analysis:

1. Date Formatting:
   - Standardized inconsistent date formats (e.g., MM/DD/YYYY and DD/MM/YYYY) into a uniform format using BigQuery's SAFE.PARSE_DATE function.

2. Handling Missing Values:
   - Replaced missing values in the Quantity_Sold column with 0, assuming no sales were made for those records.

   - Imputed missing values in the Unit_Price column with the average unit price to maintain the integrity of the total sales calculations.

3. Data Entry Errors:
   - Cleaned non-numeric characters (e.g., $ signs) from the Unit_Price column using regular expressions and converted the column to numeric data.

4. Removing Duplicate Entries:
   - Checked for and removed duplicate entries to avoid skewing the analysis.

5. Calculating Cleaned Total Sales:
   - Created a new column, Cleaned_Total_Sales, by multiplying the cleaned Unit_Price and Quantity_Sold columns.

The analysis was conducted using  BigQuery, R programming, and Power BI for visualization.


![screenshot_of_visualizations](https://github.com/raifismail/E-Commerce-Sales-Data-Improving-Sales-Through-Data-Insights/blob/d19134860ff272497ad25f89a8759da29244827a/Screenshot%202024-10-16%20114313.png)


# Stakeholders
The key stakeholders for this project include:

1) E-commerce Marketing Team : To identify high-performing regions and product categories for targeted campaigns.

2) Sales and Product Teams : To gain insights into top-selling products and optimize inventory and pricing strategies.

3) Operations and Logistics : To understand regional performance and optimize resource allocation to meet demand more efficiently.

4) Business Analysts and Data Teams : To utilize insights from data trends and analysis to inform future business decisions.


# Visualizations 

1. Total Sales by Region (Stacked Column Chart):
   - This chart provided a breakdown of total sales across the regions (East, West, North, South).

2. Total Sales by Product Category (Funnel Chart):
   - The funnel chart visualized the sales across different product categories, from the most sold to the least sold.

3. Total Sales by Month (Line Chart):
   - The line chart visualized monthly sales trends over the analysis period.

4. Total Sales Trends by Region (Line Chart):
   - This additional line chart compared the total sales trends by region across different months.

# key insights and findings

1. Regional Performance:
   - The stacked column chart indicates that the East and West regions generate the highest total sales, with the South and 
     North regions trailing behind. This suggests that marketing and sales efforts should focus on expanding in South and 
     North to balance the performance.

2. Top-performing Product Categories
   - The funnel chart clearly shows that certain product categories, such as sports and Clothing, are the biggest 
     contributors to total sales. This insight suggests a need to maintain higher inventory levels for these categories and 
     potentially introduce cross-promotions with complementary products.

3. Seasonal Trends
   - The line chart for monthly sales trends reveals that sales peak during March and May, with April and June showing a 
     slight decline. This indicates that seasonal promotions or campaigns might be effective in april to febraury to boost 
     sales during slower periods.

4. Sales Trends by Region:
   - The additional line chart showing regional sales trends over time highlights that the East region consistently leads in 
     sales, followed by the West region. Both North and South regions show steady but lower growth. This suggests a need to 
     explore region-specific marketing strategies for North and South to increase sales in those areas.

# Recommendations

1. Regional Focus:
   - increase marketing efforts in the North and South regions, where sales are lower. Targeted campaigns, region-specific offers, and localized promotions could help boost sales.

2. Product Category Optimization
   -Focus on promoting high-performing categories like sports and Clothing. Consider bundling products from lower- 
    performing categories with popular items to increase cross-category sales.

3. Seasonal Promotions
   - Plan seasonal promotions ahead of expected sales peaks (e.g., in March and May) and implement strategies to mitigate 
     sales dips (e.g., during febraury and June). Offering discounts or time-limited deals in those slower months may 
     increase overall sales.

4. Expand Regional Growth Strategies
   - Explore customized campaigns for the North and South regions. Offering promotions tailored to local preferences or 
     addressing any potential logistics challenges could help improve performance in those regions.


# Conclusion

This e-commerce case study provides actionable insights into regional sales distribution, product category performance, and seasonal trends. By implementing the recommendations, the e-commerce business can increase its total revenue, optimize marketing efforts, and grow underperforming regions.

## Dataset

The dataset used for this analysis is included in this repository. You can find it[here](https://github.com/raifismail/E-Commerce-Sales-Data-Improving-Sales-Through-Data-Insights/blob/abbf93eb1a06ffb7cecbf241e4e29cb1389726d4/E-Store%20Sales%20Data%20Improving%20Sales%20Through%20Data%20Insights.csv)
   
