# Challenge Structures

- Business situation
- Challenge Question
- Expected Answer
- Hints
- Solution

## SITUATION>

### We want to see the payment date of our existing customers.

## CHALLENGE>

### Use a SELECT statement to grab the customer id of every customer the payment date and the amount

## Hints>

### use the payment table

## Solution>

```sql
SELECT customer_id, amount, payment_date FROM payment;
```

## Expected Answer>(first 10 rows)

| 341 | 7.99 | "2007-02-15 22:25:46.996577"|
| 341 | 1.99 | "2007-02-16 17:23:14.996577"|
| 341 | 7.99 | "2007-02-16 22:41:45.996577"|
| 341 | 2.99 | "2007-02-19 19:39:56.996577"|
| 341 | 7.99 | "2007-02-20 17:31:48.996577"|
| 341 | 5.99 | "2007-02-21 12:33:49.996577"|
| 342 | 5.99 | "2007-02-17 23:58:17.996577"|
| 342 | 5.99 | "2007-02-20 02:11:44.996577"|
| 342 | 2.99 | "2007-02-20 13:57:39.996577"|
| 343 | 4.99 | "2007-02-16 00:10:50.996577"|
