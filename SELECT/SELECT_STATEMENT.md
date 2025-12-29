## What is SELECT statement

- It is used to retrieve data from one or more database tables
- you can specify your needs (ex. specific columns, tables or data that meets a specific condition)

Syntax>> SELECT column_name FROM table_name

## Database

```ascii
╔═══════════╗      ╔═══════════╗      ╔═══════════╗
║  Table-1  ║      ║  Table-2  ║      ║  Table-3  ║
╠═══╦═══╦═══╣      ╠═══╦═══╦═══╣      ╠═══╦═══╦═══╣
║c_1║c_2║c_3║      ║c_1║c_2║c_3║      ║c_1║c_2║c_3║
╠═══╬═══╬═══╣      ╠═══╬═══╬═══╣      ╠═══╬═══╬═══╣
║ g ║ 54║ a ║      ║ 1 ║ p ║ r ║      ║ r ║ 8 ║ 78║
╠═══╬═══╬═══╣      ╠═══╬═══╬═══╣      ╠═══╬═══╬═══╣
║ t ║ 67║ b ║      ║ 2 ║ y ║ w ║      ║ b ║ 9 ║ 99║
╠═══╬═══╬═══╣      ╠═══╬═══╬═══╣      ╠═══╬═══╬═══╣
║ m ║ 89║ d ║      ║ 4 ║ k ║ v ║      ║ q ║ 1 ║ 85║
╚═══╩═══╩═══╝      ╚═══╩═══╩═══╝      ╚═══╩═══╩═══╝

```

### To retrieve data from Table1 column1

```SQL
SELECT c_1 FROM Table-1
```

### How about two columns from Table3

```SQL
SELECT c_1,c_2 FROM Table-3
```

### TO select all the columns from Table2

```SQL
SELECT * FROM Table-2
```

## PRO Tips

- There is no need to capitalize SQL commands like <SELECT><FROM> etc. It works also in lower case but its always a good practice to capitalize the commands so we can see the diff. from inputs

- The best way to study a database is to use schemas
