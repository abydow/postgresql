## Purpose

- Used to filter rows in the result set after grouping and aggregation
- Useful when we filter rows based on aggregate values

## Usage

- Follows the GROUP BY clause and comes after SQL query

## Basic Syntax

```SQL
SELECT c1, aggregate_function(c2)
FROM table
GROUP BY c1
HAVING <condition>;
```

## NEED

- While WHERE clause filters individual rows before grouping, the having clause filters groups based on aggregate results

- Helps to filter out groups based on a certain condition
