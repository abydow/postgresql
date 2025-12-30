## CHALLENGE

1. Situation
2. SQL Challenge
3. Expected Results
4. Hints
5. Solution

### Situation:-

You are a data analyst working for the same video rental store. The management has noticed that some customers have similar names, and they want you to identify unique first names across all customers in the database.

### SQL Challenge:-

Write an SQL query to retrieve all distinct first names of customers from the "customer" table.

### Expected Result:-

Results in a list of Unique first names from the "customer" table, without any specific sorting

---

"Danny"
"Amber"
"Johnnie"
"Edward"
"Cindy"
"Amy"
"Earl"
"Rene"
"Geraldine"
"Carolyn"

---

### Hints:-

Use SELECT statement with DISTINCT clause to retrieve unique values

### SOlution:-

```SQL
SELECT DISTINCT (first_name) FROM customer;
```
