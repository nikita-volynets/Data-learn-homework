# Module 2 - Homework

### KPI

1. Overview

```sql
SELECT
	SUM(profit) profit,
	SUM(sales) sales,
	AVG(discount) avg_discount,
	COUNT(DISTINCT customer_id) customers,
	SUM(sales)/COUNT(DISTINCT customer_id) sales_per_customer,
	COUNT(DISTINCT order_id) orders,
	ROUND( SUM(profit)/COUNT(DISTINCT order_id),1) profit_per_order
FROM orders
WHERE EXTRACT(YEAR FROM order_date) = 2019 AND EXTRACT(MONTH FROM order_date) = 9;
```

2. Sales and Profit dynamic

```sql

```

3. Profit by Representative

```sql

```

4. Sales and Profit by Category

```sql

```

5. TOP-5 Clients in each segment by Sales

```sql

```
6. Profit by the US states

```sql

```
