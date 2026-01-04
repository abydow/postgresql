## General USe

- To restrict the rows returned by a Query
- Allows to specify maximum no. of rows to be included in the result set
- Useful in working with large databases

## Syntax

```SQL
SELECT * FROM table_name
LIMIT number_of_rows;
```

## How it works

specify the number of rows you want in the output and after applying all conditions it will only retrieve the first _n_ number of rows _( n --> your specified number )_

## Importance

1. While working with large databases fetching all rows makes the database slow and uses significant resources. USing limit allows you to fetch data thats only necessary and improves performance.

2. Helps in pagination
3. Reduces waste of memory and network resources
