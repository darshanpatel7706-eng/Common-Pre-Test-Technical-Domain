# Section A: Data Analysis & Science

## Q1. Handling Missing Age Data
If 15% of values in the Age column are missing, I would first analyze the data distribution.
I would handle the missing values by:
- Filling with median age (preferred if outliers exist)
- Using group-based averages (location or income)

This helps maintain data integrity without losing records.

## Q2. Frequently Purchased Products
To identify products frequently bought together, I would use *Market Basket Analysis*.

Techniques:
- Apriori Algorithm
- Association Rules (Support, Confidence, Lift)

Tools:
- Python (mlxtend)
- SQL


## Q3. Bar Chart vs Histogram
- *Bar Chart* is used for categorical data such as product names or cities.
- *Histogram* is used for continuous data such as age or salary.

A histogram shows data distribution, while a bar chart shows comparison.


## Q4. SQL Query
sql
SELECT customer_id, SUM(amount) AS total_spent
FROM orders
WHERE city = 'New York'
AND order_date BETWEEN '2024-01-01' AND '2024-01-31'
GROUP BY customer_id
HAVING total_spent > 500
ORDER BY total_spent DESC;


## Q5. Website Page Load Issue

Possible reasons for increased page load time:
Server overload
Inefficient database queries
Network bandwidth limitations

To investigate, I would:
Monitor server performance
Perform load testing
Optimize database queries
