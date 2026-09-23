# SQL-Analytics-and-Sales-Performance


Introduction


Structured Query Language (SQL) is one of the most important tools used in data analytics for extracting, filtering, transforming, aggregating, and analyzing relational data.
This project demonstrates the practical application of SQL to a retail-style dataset containing information about customers, products, and sales transactions. The analysis was designed around 20 business questions covering customer demographics, product categories, transaction quantities, discounts, sales performance, profitability, and customer segmentation.

The objective of this project was not only to retrieve information from the database but also to demonstrate how SQL can be used to answer practical business questions and support data-driven decision-making.

The analysis uses SQL techniques including:

SELECT
FROM
WHERE
NOT
LIKE
Comparison operators
AND
BETWEEN
GROUP BY
ORDER BY
LIMIT
COUNT()
SUM()
AVG()
MIN()
MAX()
Subqueries
SQL aggregate functions such as AVG, SUM, MIN, MAX, and COUNT are designed to calculate summary values across sets of rows.




<img width="1454" height="822" alt="SQL 1" src="https://github.com/user-attachments/assets/7e1280d9-05a5-48f9-978e-6ad59276d0f5" />

<img width="1203" height="809" alt="SQL 2" src="https://github.com/user-attachments/assets/6b6a9869-5510-4995-bcea-6bfa26977739" />

<img width="1450" height="792" alt="QL 3" src="https://github.com/user-attachments/assets/71a3b071-18ab-42ff-8bc3-db93c1c8b827" />

<img width="1371" height="199" alt="SQL 4" src="https://github.com/user-attachments/assets/45f6b356-30d3-46f3-bd3b-97c5c60bb1ad" />





Project Objective

The primary objective of this SQL project was to investigate the customer, product, and sales tables and answer specific business questions.

The analysis focused on five major areas:

Customer Analysis
Customer location
Customer age
Customer segmentation
Customer name patterns
Product Analysis
Product categories
Product-name patterns
Sales Analysis
Quantity purchased
Sales value
Profit
Discounts
Transaction dates
Statistical Analysis
Average profit
Total sales
Minimum and maximum quantities
Average sales for selected transactions
Business Analysis
High-sales/low-profit transactions
Above-average customers
Above-average profit transactions
Top-performing sales records




Dataset Structure
The analysis uses three main tables:

Customer Table
The customer table contains information relating to individual customers.

Relevant fields used in this analysis include:

customer_name
age
state
country
segment
Product Table
The product table contains information about products sold.

Relevant fields include:

product_name
category
Sales Table
The sales table contains transaction-level information.

Relevant fields include:

quantity
sales
profit
discount
order_date
The three tables provide different perspectives of the business: who the customers are, what products are being sold, and how the transactions are performing.






<img width="969" height="646" alt="SQL Analytics Dashboard" src="https://github.com/user-attachments/assets/8cceafa1-526c-413a-bff6-c79dabc9bbd0" />










Pre-Analysis
Before executing the queries, several analytical questions were identified.

Customer Questions
Where are customers located?
How many customers belong to each segment?
What is the average customer age?
Which customers are older than the average?
How many customers are located outside the United States?
Product Questions
Which products are outside the Technology category?
Which products match a particular keyword?
Which product categories may require additional investigation?
Sales Questions
What is the total sales value?
What is the average profit?
What are the minimum and maximum quantities purchased?
Which transactions have high sales but low profit?
Which transactions received large discounts?
Which transactions generated above-average profit?
These questions provided the analytical framework for the SQL investigation.




In-Analysis
The SQL analysis revealed several important analytical dimensions that can be explored further.

Customer Distribution
The customer queries examine geographic location, age, and customer segment.

This allows the dataset to be viewed not simply as a collection of transactions but as a customer population with identifiable demographic and geographic characteristics.

Transaction Behavior
Quantity-based queries help identify purchasing patterns.

Transactions involving fewer than three units can be compared with transactions involving more than five units to investigate differences in sales values.

Sales and Profitability
One of the most important analytical relationships in the project is the relationship between sales and profit.

QN 4 specifically identifies transactions where sales are relatively high but profit is relatively low.

This is important because high revenue does not automatically mean high profitability.

Discount Analysis
Transactions with large discounts can be investigated alongside profit.

A useful extension would be to compare:

Discount → Sales → Profit
to determine whether high discounts are associated with lower profit margins.





Post-Analysis Observations
Based on the SQL questions and analytical structure, several insights can be derived from the dataset once the queries are executed.

1 — Revenue and Profit Should Be Evaluated Separately
Sales value and profit measure different aspects of business performance.

A transaction can have a high sales value while producing relatively low profit.

Therefore, evaluating sales alone may provide an incomplete picture of business performance.

2 — Discounting Requires Profitability Monitoring
Transactions receiving high discounts should be analyzed alongside their profit values.

Discount strategies can potentially increase sales volume while simultaneously reducing profitability.

3 — Customer Segmentation Supports Targeted Analysis
Grouping customers by segment provides a foundation for understanding the composition of the customer base.

Different customer segments can subsequently be compared based on sales, purchasing quantity, and profitability.

4 — Average Metrics Provide Useful Benchmarks
Average age, average sales, and average profit provide reference points against which individual records can be compared.

5 — High-Quantity Transactions Deserve Further Investigation
The average sales value for transactions with quantities greater than five can be compared with the overall average sales value to determine whether larger purchases correspond with larger transaction values.




Recommendations
Based on the analytical framework developed in this project, the following areas should be investigated further.

1. Monitor High-Sales/Low-Profit Transactions
Management should investigate transactions with high sales but low profit to determine whether pricing, discounts, product costs, or other factors are affecting profitability.

2. Evaluate Discount Effectiveness
Discount levels should be compared with both sales and profit to determine whether discounts are generating sufficient commercial value.

3. Analyze Customer Segments Separately
Customer segments should be evaluated individually to understand differences in purchasing behavior and profitability.

4. Investigate High-Quantity Purchases
Large-quantity transactions could be analyzed to determine which products and customer segments are responsible for high-volume purchases.

5. Expand Geographic Analysis
Customer location can be analyzed by state and country to identify geographic patterns in the customer base.

6. Develop a Profitability Dashboard
The SQL outputs could be connected to a visualization tool such as Power BI or Tableau to create an interactive dashboard containing:

Total Sales

Total Profit

Average Profit

Number of Transactions

Average Discount

Customer Segments

Sales by Category

Profit by Category

Sales by Region

High-Sales/Low-Profit Transactions






Conclusion
This SQL project demonstrates how relational data can be transformed into meaningful business information through structured querying.

The analysis covered customer demographics, geographic distribution, product categories, transaction quantities, sales values, discounts, and profitability.

A key analytical theme throughout the project is the distinction between sales performance and profitability. Rather than focusing solely on revenue, the analysis also investigates profit, discounts, transaction quantity, and above-average performance.

The project also demonstrates the importance of using SQL correctly. Small syntax or logic errors can change the meaning of an analysis. For example, ordering by profit instead of sales would answer a different question, while placing the WHERE clause incorrectly can prevent a query from executing.

Overall, the project provides a practical demonstration of SQL as an analytical tool for converting raw customer, product, and transaction data into information that can support business analysis and decision-making.



