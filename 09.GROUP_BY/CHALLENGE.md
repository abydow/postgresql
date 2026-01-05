## CHALLENGE 1

- Find the total amount collected by each staff member

### Solution

```SQL
SELECT staff_id, SUM(amount) FROM payment
GROUP BY staff_id
ORDER BY COUNT(amount)
```

### Result

1 30252.12
2 31059.92

## CHALLENGE 2

- List all payments made on a specific date

```SQL
SELECT payment_id, amount, payment_date FROM payment
WHERE DATE(payment_date) = '2007-02-16';
```
