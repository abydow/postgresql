## Basic Info

- Special functions that perform calculations on a set of values and returns a single value in result
- Summarizes meaningful insights from large data sets in a database
- Works on a group of rows and returns a single value for each group
- Crucial for calculating avg., sums, counts, min. and max. values and more

## key aspects

1. Often used in conjunction with Group by clause
2. most common aggregate functions -->

- SUM - sum of numeric column in a group
- AVG - Average of numeric column in a group
- COUNT - number of rows in a group
- MIN - minimum value of a numeric column from a group
- MAX - maximum value of a numeric column from a group

---

_NOTE_ - ROUND() is a scalar function. not a aggregate function

- example

```SQL
SELECT ROUND(price, 2/*how many numbers you want after "."*/) FROM products;
```

---

## USE

```SQL
SELECT MAX(column1),MIN(column2),....
FROM table1
```
