## General Use

- Sorts the result set of a query in a specified order
- Makes the query easier to interpret

## Reason to use it

1. Represents the data in a logical and readable order
2. Sorting the result makes it easier for analysis and identification (trends, outliers or patterns)
3. When dealing with large datasets, we can implement pagination to show only a subset
   of a data on each page. Proper sorting is essential to ensure consistency between pages.

## Syntax

```SQL
SELECT COLUMN1, COLUMN2, .....
FROM table_name
WHERE <condition>
ORDER BY COLUMN1[ASC|DESC],COLUMN2[ASC|DESC],......;
```

## How it works

The column that needs to be sorted will be specified in here . we can sort multiple columns and for each column we have to specify the order Ascending(default) or descending
