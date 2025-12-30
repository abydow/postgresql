## Intro:-

- It is used to filter the result set of a query
- It also retrieves only unique rows from specified column or comb. of columns
- Particularly useful when someone wants to remove duplicate records from query results

## Syntax:-

```SQL
SELECT DISTINCT column FROM table_name;
```

> Or to make it more clear

```SQL
SELECT DISTINCT (column) FROM table_name;
```

## How DISTINCT statement works:-

1. Executes as usual, fetching data from specified table or tables
2. Removes duplicates from result set of the column
3. First occurrence of each unique combination of values

employees

```ascii
╔══════════════╦═════════════╦════════════╦═════════════╗
║ employee_id  ║ first_name  ║ last_name  ║ department  ║
╠══════════════╬═════════════╬════════════╬═════════════╣
║      1       ║    John     ║   Smith    ║     HR      ║
╠══════════════╬═════════════╬════════════╬═════════════╣
║      2       ║    Jane     ║    Doe     ║     IT      ║
╠══════════════╬═════════════╬════════════╬═════════════╣
║      3       ║    John     ║   Smith    ║     HR      ║
╠══════════════╬═════════════╬════════════╬═════════════╣
║      4       ║    Alice    ║  Johnson   ║     HR      ║
╚══════════════╩═════════════╩════════════╩═════════════╝
```

## If we use SELECT DISTINCT in employees table

```SQL
SELECT DISTINCT first_name,last_name FROM employees
```

### The result>>

```ascii
╔══════════════╦═════════════╗
║ first_name   ║ last_name   ║
╠══════════════╬═════════════╣
║ John         ║ Smith       ║
╠══════════════╬═════════════╣
║ Jane         ║ Doe         ║
╠══════════════╬═════════════╣
║ Alice        ║ Johnson     ║
╚══════════════╩═════════════╝
```
