## Count Function in SQL>>

1. It is an _AGGREGATE FUNCTION_
2. Lets us count the number of rows that match a specified condition within a table or a result set.

3. Returns a single value representing the count of rows that meet the criteria.

## USE>>

- Used for data analytics
- helps to fetch statistical data

## Example>>

```ascii
╔════════╦══════════╦═════════════╗
║ emp_id ║ emp_name ║ dep         ║
╠════════╬══════════╬═════════════╣
║   1    ║ John     ║ HR          ║
╠════════╬══════════╬═════════════╣
║   2    ║ Alice    ║ IT          ║
╠════════╬══════════╬═════════════╣
║   3    ║ Bob      ║ Finance     ║
╠════════╬══════════╬═════════════╣
║   4    ║ Emily    ║ HR          ║
╠════════╬══════════╬═════════════╣
║   5    ║ Michael  ║ IT          ║
╚════════╩══════════╩═════════════╝
```

---

### To count all the "employees" in the table

- Syntax :

```SQL
SELECT COUNT(*) FROM employees;
```

- Output:

```ascii
╔═════════════╗
║    Count    ║
╠═════════════╣
║      5      ║
╚═════════════╝
```

---

### Count the number of unique departments in the "employees" table

- Syntax :

```SQL
SELECT COUNT(DISTINCT department) FROM employees;
```

- Output:

```ascii
╔═════════════╗
║    Count    ║
╠═════════════╣
║      3      ║
╚═════════════╝
```

**Note**: Use COUNT(\*) to count the no. of rows and use COUNT(row_name) to avoid null values and to count the no. of entries.
