## SQL Project: Supermarket Sales Analysis

### Overview:
This project involved using MySQL Workbench to analyze extensive sales data from a supermarket, aiming to uncover insights into revenue generation, identify top-selling branches, and segment customers. I examined popular products and payment methods while analyzing sales trends to understand seasonal patterns and growth trajectories.

Additionally, this technical report presents a series of SQL queries crafted to analyze a dataset with detailed sales transaction information. By employing various SQL techniques, we explored the data to identify significant trends, patterns, and anomalies. The results provided valuable insights into customer behavior, product performance, and overall business performance.


### Analysis:
1. **Count the total number of invoices:** Calculated the total number of invoices generated from the sales data in the table.
```
SELECT COUNT(*) AS total_invoices
FROM sales_data;
```

2. **Total Revenue Calculation:** Calculated the total revenue generated from the sales data in the table.
```
SELECT SUM(Total) AS total_revenue
FROM sales;
```

3. **Top-Selling Branch Identification:** Identified the branch (city) with the highest total sales revenue.
```
SELECT Branch, City, SUM(Total) AS total_revenue
FROM sales
GROUP BY Branch, City
ORDER BY total_revenue DESC
LIMIT 1;
```

4. **Find all invoices from the city of Yangon:** Identified the city (Yangon) total no of invoices.
```
SELECT *
FROM sales_data
WHERE City = 'Yangon';
```

5. **Customer Segmentation by Type:** Determined the number of sales made to members and normal customers.
```
SELECT Customer_type, COUNT(*) AS num_sales
FROM sales
GROUP BY Customer_type;
```

6. **Find the top 10 customers by total spending:** Determined the top 10 customers.
```
SELECT Customer_type, SUM(Total) AS total_spent
FROM sales_data
GROUP BY Customer_type
ORDER BY total_spent DESC
LIMIT 10;
```

7. **Top Gross Income Generating Product Line:** Identified the product line that generated the highest gross income and its total.
```
SELECT Product_line, SUM(gross_income) AS total_gross_income
FROM sales
GROUP BY Product_line
ORDER BY total_gross_income DESC
LIMIT 1;
```
8. **Average Unit Price by Branch:** Calculated the average unit price of products sold in each branch.
```
SELECT Branch, City, AVG(Unit_price) AS avg_unit_price
FROM sales
GROUP BY Branch, City;
```
9. **Most Popular Payment Method:** Identified the most popular payment method among customers.
```
SELECT Payment, COUNT(*) AS num_payments
FROM sales
GROUP BY Payment
ORDER BY num_payments DESC
LIMIT 1;
```
10. **Average Gross Margin Percentage by Product Line:** Calculated the average gross margin percentage for each product line.
```
SELECT Product_line, AVG(gross_margin_percentage) AS avg_margin_percentage
FROM sales
GROUP BY Product_line;
```
11. **Day with Highest Sales Volume:** Determined the day of the week with the highest sales volume.
```
SELECT IFNULL(DAYNAME(Date), 'Unknown') AS day_of_week, COUNT(*) AS num_sales
FROM sales
GROUP BY DAYNAME(Date), Date
ORDER BY num_sales DESC
LIMIT 1;
```
12. **Total Quantity Sold by Product Line:** Calculated the total quantity sold for each product line.
```
SELECT Product_line, SUM(Quantity) AS total_quantity_sold
FROM sales
GROUP BY Product_line;
```
13. **Total Tax Amount Collected by Gender:** Calculated the total tax amount collected for each gender.
```
SELECT Gender, SUM(COALESCE(`Tax_5%`, 0)) AS total_tax_amount
FROM sales
GROUP BY Gender;
```

14. **Find the total revenue generated by each branch** Calculated the total revenue generated by each gender.
```
SELECT Branch, SUM(Total) AS total_revenue
FROM sales_data
GROUP BY Branch;
```

15. **Join the sales data with customer data to find the total revenue generated by each customer type:** 
SELECT s.Customer_type, SUM(s.Total) AS total_revenue
FROM sales_data s
JOIN customers c ON s.Customer_type = c.Customer_type
GROUP BY s.Customer_type;

### Conclusion:
Through this analysis, valuable insights were obtained regarding sales performance, customer behavior, and product popularity. These insights can be used to optimize marketing strategies, inventory management, and customer targeting to enhance overall business performance.
1. **Total Revenue Calculation:** This query gives an overview of the overall sales performance.
2. **Top-Selling Branch Identification:** Identifying the branch with the highest sales revenue provides insights into geographical sales distribution.
3. **Customer Segmentation by Type:** Understanding the distribution of sales between member and normal customers can be crucial for marketing and loyalty programs.
4. **Top Gross Income Generating Product Line:** Identifying the product line that generates the highest gross income provides insights into product performance and profitability.
5. **Average Unit Price by Branch:** Calculating the average unit price by branch helps in understanding pricing strategies and regional preferences.
6. **Most Popular Payment Method:** Identifying the most popular payment method offers insights into customer payment preferences and can inform payment processing strategies.
7. **Average Gross Margin Percentage by Product Line:** Calculating the average gross margin percentage by product line provides insights into product profitability and can inform pricing and marketing strategies.
8. **Day with Highest Sales Volume:** Identifying the day of the week with the highest sales volume helps in understanding sales patterns and can inform staffing and inventory management.
9. **Total Quantity Sold by Product Line:** Understanding the total quantity sold for each product line helps in assessing product demand and inventory management.
10. **Total Tax Amount Collected by Gender:** Calculating the total tax amount collected by gender provides insights into spending patterns and can inform marketing strategies.