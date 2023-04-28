# Module 2 - Homework

Installed Postgres BD, DBeaver and created tables with Superstore data (I used sample file with sql query).

### 1. KPI

Wrote queries to find KPIs from Module 1.

**1.1 Overview**

```sql
SELECT
	SUM(profit) profit,
	SUM(sales) sales,
	AVG(discount) avg_discount,
	COUNT(DISTINCT customer_id) customers,
	SUM(sales)/COUNT(DISTINCT customer_id) sales_per_customer,
	COUNT(DISTINCT order_id) orders,
	ROUND( SUM(profit)/COUNT(DISTINCT order_id),1) profit_per_order
FROM orders o
WHERE EXTRACT(YEAR FROM order_date) = 2019 AND EXTRACT(MONTH FROM order_date) = 9;
```

**1.2 Sales and Profit dynamic**

```sql
SELECT
	EXTRACT(YEAR FROM order_date) year_date,
	EXTRACT(MONTH FROM order_date) month_date,
	SUM(sales),
	SUM(profit)
FROM orders o 
GROUP BY EXTRACT(YEAR FROM order_date), EXTRACT(MONTH FROM order_date)
ORDER BY year_date, month_date ;
```

**1.3 Profit by Representative**

```sql
SELECT 
	p.person,
	SUM(profit) profit
FROM orders o 
LEFT JOIN people p ON p.region  =o.region
WHERE EXTRACT(YEAR FROM order_date) = 2019 AND EXTRACT(MONTH FROM order_date) = 9
GROUP BY p.person
ORDER BY profit DESC;
```

**1.4 Sales and Profit by Category**

```sql
SELECT DISTINCT 
	segment ,
	category ,
	SUM(sales) sales,
	SUM(profit) profit
FROM orders o
GROUP BY segment , category  
ORDER BY segment ; 
```

**1.5 TOP-5 Clients in each segment by Sales**

```sql
WITH new_table AS (

(SELECT DISTINCT 
	segment,
	customer_name  ,
	SUM(sales) sales
FROM orders o
GROUP BY segment , customer_name  
HAVING segment = 'Consumer'
ORDER BY sales DESC
LIMIT 5)

UNION 

(SELECT DISTINCT 
	segment,
	customer_name ,
	SUM(sales) sales
FROM orders o
GROUP BY segment , customer_name  
HAVING segment = 'Corporate'
ORDER BY sales DESC
LIMIT 5)

UNION

(SELECT DISTINCT 
	segment,
	customer_name ,
	SUM(sales) sales
FROM orders o
GROUP BY segment , customer_name  
HAVING segment = 'Home Office'
ORDER BY sales DESC
LIMIT 5)

)

SELECT *
FROM new_table
ORDER BY segment;
```
**1.6 Profit by the US states**

```sql
SELECT 
	country,
	state,
	SUM(profit) profit 
FROM orders o
GROUP BY country , state 
ORDER BY state;
```

### 2. Data Models

**2.1 Conceptual**


**2.2 Logical**


**2.3 Physical**



