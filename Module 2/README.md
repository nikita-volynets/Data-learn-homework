# Module 2 - Homework

### Overview - KPI

```sql
SELECT 
	SUM(profit) profit,
	SUM(sales) sales,
	AVG(discount) avg_discount,
	COUNT(DISTINCT customer_id) customers,
	SUM(sales)/count(DISTINCT customer_id) sales_per_customer,
	COUNT(DISTINCT order_id) orders,
	SUM(profit)/COUNT(DISTINCT order_id) profit_per_order
FROM orders
```
