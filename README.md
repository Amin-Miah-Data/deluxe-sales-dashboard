Deluxe Revenue and Profit Dashboard

📋 Project Overview

This project analyses two years of sales data for Deluxe, a UK-based online retailer, covering January 2019 to December 2020. Starting from a raw dataset, I cleaned and structured the data, built PivotTables to summarise key metrics, and designed an interactive Excel dashboard to answer one business question: which product categories and countries drive the most revenue and profit?

📸 Dashboard Preview

<img width="1720" height="734" alt="dashboard_screenshot" src="https://github.com/user-attachments/assets/936a244b-078b-41e3-83dc-73cdf981820f" />














🎯 Objectives

- Identify the top performing product categories by revenue and profit
- Identify the top performing countries by revenue
- Understand customer purchasing behaviour by device type
- Build an interactive dashboard to support data-driven decision making

📂 Data Source

- Dataset: Deluxe Sales Export 2019-2020
- Source: Kaggle
- Records: 1,000 orders
- Key fields: country, order value (EUR), cost, date, category, device type, sales manager, sales representative, order ID

🧹 Data Cleaning

All cleaning was done in Excel before analysis began:

- No duplicate records found
- No missing or blank values found
- Fixed date formatting - some dates were stored as text and converted to proper date format using Text to Columns
- Fixed cost column - some values were stored as text rather than numbers
- Validated revenue, cost, and profit columns - no negative or zero values found
- Checked category and country columns for inconsistencies - none found
- Added a profit column (order value minus cost) across all 1,000 rows
- Added a year column using the YEAR function to enable slicer filtering

🔢 Calculations

- Profit per order - =B2-C2 applied across all 1,000 rows
- Year - =YEAR(D2) extracted from the date column to enable year filtering
- Total Revenue - ='Revenue by Category'!B12 pulling the grand total from the PivotTable
- Total Profit - ='Profit by Category'!B12 pulling the grand total from the PivotTable
- Total Orders - =COUNTA(Data!J2:J1001) counting all order IDs
- Top Category - Clothing, identified from the Revenue by Category PivotTable sorted largest to smallest

📌 Key Metrics

- Total Revenue: €113,361,738.71
- Total Profit: €18,992,427.72
- Total Orders: 1,000
- Top Category: Clothing

📊 Dashboard Features

- Four KPI cards showing total revenue, total profit, total orders, and top category
- Revenue by Category - horizontal bar chart
- Revenue by Top 10 Countries - column chart
- Profit by Category - column chart
- Revenue by Device Type - doughnut chart
- Year and category slicers connected to all charts for dynamic filtering

🛠️ Tools and Technologies

- Microsoft Excel - data cleaning, exploratory analysis, and dashboard design
- PivotTables - data summarisation and aggregation
- PivotCharts - data visualisation
- Excel slicers - interactive filtering across all charts

💡 Insights and Findings

- Clothing is the top category by both revenue (17.7M EUR) and profit (2.9M EUR), making it the most commercially valuable product line
- Games, Appliances, and Electronics are strong mid-tier performers, each generating over 14M EUR in revenue
- Accessories and Other are the weakest categories at 4.7M EUR and 3.3M EUR, with limited commercial contribution
- Portugal leads all countries at 27.8M EUR, ahead of France (25.9M EUR) and Sweden (19.6M EUR)
- The UK sits fourth at 12.1M EUR despite being the retailer's home market, suggesting an untapped domestic opportunity
- 79% of purchases are made on PC, with Mobile at 14% and Tablet at 7%, indicating the customer base skews heavily desktop

✅ Recommendations

- Prioritise Clothing and Games for continued investment given their strong and consistent performance across both revenue and profit
- Review Accessories and Other to determine whether repositioning or discontinuation is the right commercial decision
- Investigate why the UK underperforms relative to Portugal and France and develop a targeted domestic growth strategy
- Explore mobile experience improvements given that over one in five customers shop on a non-PC device
