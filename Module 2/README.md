# Module 2 - Homework

## Overview - KPI

```sql
SELECT sum(profit) profit,
	sum(sales) sales,
	avg(discount) avg_discount,
	count(DISTINCT customer_id) customers,
	sum(sales)/count(DISTINCT customer_id) sales_per_customer,
	COUNT(DISTINCT order_id) orders,
	sum(profit)/COUNT(DISTINCT order_id) profit_per_order
FROM orders
```
