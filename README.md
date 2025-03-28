# PBI-Sales
The Global Superstore Sales project utilizes a dataset containing detailed records of worldwide sales activities for the fictional Superstore company. This project aims to design an interactive dashboard that provides senior management with insights into business performance, aiding in market expansion and strategic product decisions.
# Introduction
The Global Superstore Sales project provides senior management with key insights into global operations. Superstore, a multinational company offering office supplies, furniture, and technology, operates in diverse markets with complex sales patterns.

This project helps stakeholders identify high-potential regions and profitable product categories, while addressing return trends and customer feedback to improve efficiency and satisfaction. Through a visually rich dashboard, it transforms raw data into strategic insights, supporting informed decision-making and future growth.
# Objectives
- Identify the most profitable regions and markets, supporting data-driven decisions for market expansion.

- Analyze product performance to determine strategic product categories and optimize inventory management.

- Provide actionable insights into return patterns to address customer satisfaction and reduce return rates.
# Processing
## Data Collection and Data Cleaning
This project utilizes three interconnected tables—Orders, People, and Returns—to provide a comprehensive view of Superstore's global operations. The Orders table records detailed sales transactions, enabling analysis of product demand, regional performance, and sales trends. The People table contains information on sales representatives, helping assess workforce impact and regional sales effectiveness. The Returns table tracks product returns, offering insights into customer satisfaction and operational issues.

Before analysis, the data underwent thorough cleaning to ensure accuracy and consistency. Missing values in product names, order dates, and returns were addressed; duplicates and discrepancies in sales and representative records were resolved. These preparation steps ensured a reliable dataset for building insightful, data-driven visualizations in Power BI.
## Data Transformation:
After cleaning, the data was transformed for analysis by standardizing formats and calculating key metrics like regional sales performance, return rates, and fulfillment times. Products were categorized by location and quality to reveal regional preferences and return patterns, enabling more detailed segmentation.

To optimize Power BI performance, dimensional tables (e.g., Dim_Categories, Dim_Sub-Categories, Dim_Product, and Dim_Locations) were created by extracting relevant attributes. This reduced redundancy and improved data organization for efficient analysis.

![Relationship_Tables.png](https://github.com/khangtran85/Business-Performance-Analysis-for-Sales/blob/main/Relationship_Tables.png)
## Data Modeling:
A relational data model was built to integrate the Orders, People, and Returns tables, enabling dynamic filtering and real-time insights in Power BI. This allowed users to explore sales trends, regional performance, and return rates across connected data sources for more informed decisions.

The model uses a snowflake schema, with normalized dimensions like Dim_Sub-Categories linked to Dim_Categories. The central Fact_Orders table stores key metrics such as sales and orders, supporting hierarchical analysis across products, categories, and regions.

![Snowflake_Model.png](https://github.com/khangtran85/Business-Performance-Analysis-for-Sales/blob/main/Snowflake_Model.png)

The snowflake schema offers key advantages by reducing data duplication and ensuring consistency, especially in large, hierarchical datasets. Its structured design improves Power BI’s loading speed and supports scalability for future data expansion.

This efficiency enables stakeholders to quickly access insights, explore data intuitively, and focus on critical metrics like regional sales and product performance for timely, informed decision-making.
## Design Thinking
### Step 1: Empathize
### Step 2: Define Point of View
### Step 3: Ideate
### Stage 4: Prototype and Review
## Visualization Development
The visualization in Power BI was carefully designed to deliver actionable insights through four distinct pages, each tailored to address critical aspects of the company's operations.

**Overview:** This page provides a comprehensive summary of the company's overall business performance. Key metrics such as total revenue, profit margins, segment and regional performance are displayed in an intuitive layout, offering stakeholders a high-level understanding of the company's current standing.

![Overview.png](https://github.com/khangtran85/Business-Performance-Analysis-for-Sales/blob/main/Overview.png)

**Sub/Category Detail:** This page dives deeper into the performance of individual product categories and sub-categories. Visuals such as bar charts, pie charts, and trend lines illustrate profit, revenue, and other indicators. By identifying the strengths and weaknesses of specific product segments, this page empowers decision-makers to refine their product strategies and focus on high-performing categories.

![Sub_Category Detail.png](https://github.com/khangtran85/Business-Performance-Analysis-for-Sales/blob/main/Sub_Category%20Detail.png)

**Seller:** Focused on sales representatives, this page evaluates their contributions across various markets. Metrics like total sales, regional performance, and individual efficiency are analyzed. These insights highlight top-performing sellers, identify areas needing improvement, and guide strategies to maximize sales team effectiveness.

![Seller.png](https://github.com/khangtran85/Business-Performance-Analysis-for-Sales/blob/main/Seller.png)

**Returned:** Dedicated to analyzing product returns, this page examines return rates, reasons for returns, and their impact on overall performance. Insights drawn from this data help pinpoint recurring issues, such as product quality or delivery discrepancies, and suggest actionable steps to reduce returns and enhance customer satisfaction.

![Returned.png](https://github.com/khangtran85/Business-Performance-Analysis-for-Sales/blob/main/Returned.png)
# Recommendation
The analysis of Superstore’s data provides critical insights to drive strategic decision-making in alignment with the company's objectives. First, identifying the most profitable regions and markets reveals significant opportunities for targeted market expansion. Regions with consistently high revenue and profitability should receive increased investment in marketing and distribution to strengthen their dominance, while emerging markets showing potential should be explored with tailored entry strategies.

Second, the evaluation of product performance emphasizes the importance of optimizing inventory and strategic product management. High-performing categories should be prioritized in inventory planning to prevent stockouts and capture maximum demand. Conversely, underperforming categories warrant a thorough review to identify potential issues, such as pricing inefficiencies or mismatches with customer preferences, enabling the development of targeted improvement plans.

Lastly, understanding return patterns is vital to enhancing customer satisfaction and reducing associated costs. By analyzing the root causes of frequent returns—whether due to product quality, delivery issues, or unmet expectations—the company can implement focused quality assurance measures and refine customer service processes. Such initiatives not only reduce return rates but also foster greater trust and loyalty among customers.
