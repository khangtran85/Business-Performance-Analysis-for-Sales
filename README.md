# PBI-Sales
The Global Superstore Sales project utilizes a dataset containing detailed records of worldwide sales activities for the fictional Superstore company. This project aims to design an interactive dashboard that provides senior management with insights into business performance, aiding in market expansion and strategic product decisions.
# Introduction
The Global Superstore Sales project is designed to provide senior management with actionable insights into the company’s worldwide business operations. Superstore, a multinational enterprise, operates across diverse markets, selling a broad range of products, including office supplies, furniture, and technology. With an expansive reach and varied customer base, the company faces the challenge of navigating complex sales patterns and regional market dynamics.

Senior stakeholders are particularly focused on understanding the current performance landscape to identify areas of growth and profitability. They aim to uncover which regions hold the most potential for expansion and determine which product categories offer the best opportunities for strategic investment. Moreover, the ability to interpret and act on return patterns and customer feedback is critical for improving operational efficiency and customer satisfaction.

This project aims to empower decision-makers by transforming raw data into an intuitive, visually rich dashboard. The dashboard will illuminate sales trends, highlight high-performing regions and products, and offer actionable insights to refine business strategies. By bridging the gap between data and decisions, this project will play a vital role in shaping the company’s future growth trajectory.
# Objectives
- Identify the most profitable regions and markets, supporting data-driven decisions for market expansion.

- Analyze product performance to determine strategic product categories and optimize inventory management.

- Provide actionable insights into return patterns to address customer satisfaction and reduce return rates.
# Processing
## Data Collection:
The dataset used in this project offers a comprehensive view of Superstore's global operations through three interconnected tables: Orders, People, and Returns. The Orders table records all sales transactions, including product details, quantities, revenues, and order dates, enabling an analysis of sales performance, product demand, and revenue generation over time. By examining this table, we can identify top-selling products, regional performance, and seasonal trends, helping to inform pricing, inventory management, and sales strategies.

The People table provides data on the sales representatives across different regions, shedding light on how workforce performance impacts sales outcomes. Analyzing this table allows for a better understanding of regional sales efforts and the effectiveness of individual sales reps. It helps identify areas where additional support or realignment might be necessary to boost performance in underperforming regions or enhance overall sales efficiency.

The Returns table tracks product returns, offering insights into customer satisfaction and areas for improvement in product quality or service. By analyzing return patterns, we can pinpoint products with high return rates or identify regional trends that may signal dissatisfaction or operational issues. By combining insights from all three tables, we can gain a holistic view of Superstore’s business, enabling more informed decision-making to improve sales, reduce returns, and optimize the overall customer experience.

Upload the data to Power BI using the "Transform data" tag.
## Data Cleaning:
The "Orders" table, which contains details of sales transactions, required significant data cleaning to ensure its reliability. Missing values in product names and order dates were addressed, and discrepancies between product availability and sales data were resolved. Duplicates were removed to maintain a unique dataset, ensuring accuracy in analysis. Similarly, in the "People" table, inconsistencies in regional sales representatives' data were identified and corrected to maintain consistency across the dataset. The "Returns" table, which logs returned products, also had missing values and inconsistencies that were rectified. These data cleaning efforts ensured a comprehensive and reliable dataset for further analysis.
## Data Transformation:
After addressing the data cleaning issues, the next step was to transform the data for analytical purposes. Data formats across all tables were standardized, ensuring consistency in how sales transactions, product categories, and regional information were recorded. Key metrics such as sales performance by region, product return rates, and order fulfillment times were calculated to provide actionable insights. Products in the "Orders" and "Returns" tables were categorized by location and quality status to better understand regional product preferences and return patterns. This transformation allowed for more granular analysis and easier segmentation of sales performance.

To optimize data structure and enhance performance in Power BI, additional dimensional tables such as Dim_Categorys, Dim_Sub-Categorys, Dim_Product, and Dim_Locations were created by extracting specific attributes from the original dataset. This process involves segmenting detailed data into smaller, specialized tables, which reduces redundancy and organizes the data for more efficient querying and analysis.

## Data Modeling:
The data modeling process was essential in creating a coherent and structured framework for analysis. Relationships between the "Orders," "People," and "Returns" tables were established, allowing for seamless integration of data from various sources. This relational model facilitated real-time updates and dynamic filtering in Power BI, ensuring that users could easily explore sales patterns, regional performance, and product return trends. The ability to analyze data across tables allowed for deeper insights, such as identifying underperforming regions or products with high return rates, enabling more effective decision-making for the business.

This model follows a snowflake schema, where dimensions are further normalized into sub-dimensions. For instance, Dim_Sub-Categorys connects with Dim_Categorys, offering a hierarchical structure that reflects real-world relationships among categories, sub-categories, and products. The central Fact_Orders table serves as the sole fact table, containing quantitative metrics such as sales and order data, which can be analyzed across these connected dimensions.



The benefits of this approach are significant. By separating the data into normalized dimensions, the snowflake schema reduces data duplication and ensures consistency, especially for large datasets with complex hierarchies. This structure directly enhances the loading speed in Power BI, as the reduced data size and organized relationships require fewer computational resources. Moreover, the schema supports scalability, making it easier to integrate new dimensions or extend existing ones without compromising performance.

This improved efficiency ensures that stakeholders can quickly access actionable insights, navigate data intuitively, and focus on critical metrics like sales performance by region or product category, ultimately enabling more informed and timely decision-making.
## Visualization Development:
![Overview.png](https://github.com/khangtran85/PBI-Sales/blob/main/Overview.png)

![Sub_Category Detail.png](https://github.com/khangtran85/PBI-Sales/blob/main/Sub_Category%20Detail.png)

![Seller.png](https://github.com/khangtran85/PBI-Sales/blob/main/Seller.png)

![Returned.png](https://github.com/khangtran85/PBI-Sales/blob/main/Returned.png)
# Recommendation
