## CHALLENGE 1

- Retrieve the first_name, last_name and email of all customers

### SOLUTION

```SQL
SELECT first_name, last_name, email FROM customer;
```

## CHALLENGE 2

- Retrieve the payment_id, customer_id, amount for payments with an argument greater than 100

### SOLUTION

```SQL
SELECT payment_id, customer_id, amount FROM payment
WHERE amount > 10;
```

## CHALLENGE 3

- Retrieve the first_name, last_name and email of customers, sorted by last name in ascending order, and limit the results to 5

### SOLUTION

```SQL
SELECT first_name, last_name, email FROM customer
ORDER BY last_name ASC
LIMIT 5;
```

## CHALLENGE 4

- Retrieve the payment_id, customer_id, payment_date for payments made in year 2022

### SOLUTION

```SQL
SELECT payment_id, customer_id,payment_date FROM payment
WHERE EXTRACT(year FROM payment_date) = 2022;
```

## CHALLENGE 5

- Retrieve the first_name, last_name and email of customers whose email contains 'gmail'.

### SOLUTION

```SQL
SELECT first_name, last_name, email FROM customer
WHERE email LIKE '%gmail%';
```

## CHALLENGE 6

- Retrieve the payment_id, customer_id, amount for payments with an amount between 50 and 100 (inclusive)

### SOLUTION

```SQL
SELECT payment_id, customer_id,payment_date FROM payment
WHERE amount BETWEEN 50 and 100;
```
