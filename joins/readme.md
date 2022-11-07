#### Orders 

| cust_id | id | order_date | price |
|--|--|--|--|
| 2 | 1 | 2011-01-01 | 100 |
| 2 | 2 | 2012-01-01 | 100 |
| 1 | 3 | 2022-05-05 | 200 |
| 3 | 4 | 2022-05-06 | 100 |
| 7 | 5 | 2000-01-01 | 100 |

#### Customers

| cus_id | cust_name | 
|--|--|
| 2 | Prakriti | 
| 2 | Kreetika | 
| 1 | Anit | 
| 3 | Dikshya | 


Here is an example query:

```
SELECT c.customer, o.order_date, o.price
FROM Customers as c
JOINS Orders ON o.cus_id = cust_id 
``` 

Another example: 

```
SELECT customer, order_date, price
FROM Customers
JOINS Orders ON cus_id = cust_id 
```