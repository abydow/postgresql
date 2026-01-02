## INTRO

### Where clause is important when we need to fetch certain data based on conditions

## Syntax

```SQL
SELECT Column1,Column2
From Table1
WHERE <Condition>;
```

## Basic explanation

### SELECT

#### Selects specified columns. EX -- Column1, Column2

### FROM

#### The table from where data will be retrieved

### WHERE

#### The information you need based on a condition

## Operators

- | = : Equal to
- | <> or != : Not equal to
- | > : Greater then
- | < : Less than
- | >= : Greater than or equal to
- | <= : Less than or equal to
- | BETWEEN : Between a range of values (inclusive)
- | LIKE : Pattern matching using wildcards(often used with % and \_)
- | IN : Matches any value in list
- | IS NULL : Checks for NULL values
- | AND, OR, NOT : Logical operators for combining multiple conditions

## USE

```ascii
+-------------+------------+-----------+-------------+-----+--------+------------+------------+--------+--------------+
| employee_id | first_name | last_name |  job_title  | age | salary | department | experience | rating | phone_number |
+-------------+------------+-----------+-------------+-----+--------+------------+------------+--------+--------------+
|      1      |    John    |    Doe    |   Manager   |  35 |  80000 |   Sales    |      7     |   4.5  | 555-123-4567 |
|      2      |    Jane    |   Smith   |  Supervisor |  28 |  60000 |     HR     |      5     |   4.2  | 555-987-6543 |
|      3      |   Robert   |  Johnson  |   Analyst   |  42 |  75000 |   Finance  |     10     |   4.7  |     NULL     |
|      4      |  Jennifer  |  Williams |   Manager   |  38 |  90000 |  Marketing |     12     |   4.9  | 555-444-3333 |
|      5      |   Michael  |   Brown   |  Supervisor |  32 | 650000 |   Sales    |      8     |   4.3  | 555-777-8888 |
|      6      |    Laura   |   Davis   | Coordinator |  27 | 550000 |    Admin   |      3     |   4.0  | 555-222-1111 |
|      7      |    James   |   Miller  |   Analyst   |  29 |  70000 |     HR     |      6     |   4.6  | 555-999-0000 |
|      8      |    Emily   |  Anderson |  Supervisor |  31 |  68000 |  Marketing |      7     |   4.4  | 555-999-0000 |
+-------------+------------+-----------+-------------+-----+--------+------------+------------+--------+--------------+
```

> We will use this table as an example

### Use of "="

```SQL
SELECT * FROM employees
WHERE department = "Sales";
```

> _This Query will only retrieve rows where department is Sales_. (IN OUR TABLE IT'S ROW 1 AND 5)

### Use of "<>" or "!="

```SQL
SELECT * FROM employees
WHERE department != "Finance";
```

> _This Query will only retrieve rows where department is not Finance_. (IN OUR TABLE IT'S all the rows except 3)

### Use of ">"

```SQL
SELECT * FROM employees
WHERE age>30;
```

> _This Query will only retrieve rows where age is greater than 30_.

### Use of "<"

```SQL
SELECT * FROM employees
WHERE age<30;
```

> _This Query will only retrieve rows where age is less than 30_.

### Use of ">="

```SQL
SELECT * FROM employees
WHERE experience>=5;
```

> _This Query will only retrieve rows where age is greater than or equals to 5_.

### Use of "<="

```SQL
SELECT * FROM employees
WHERE experience<=5;
```

> _This Query will only retrieve rows where age is less than or equals to 5_.

### Use of "BETWEEN"

```SQL
SELECT * FROM employees
WHERE age BETWEEN 25 AND 40;
```

> _This Query will only retrieve rows where age is between 25 and 40 (inclusive)_.

### Use of "LIKE"

---

#### For this we have to learn about use of wildcard characters "%" and "\_"

- we use wild card characters when we want to fetch strings with a certain pattern,

  for example we have four characters:-
  "John","Joe","Jack","Jason"

  Can we spot any similarity? yes the strings have one common letter "J"
  so to fetch these characters in a database of 1000 user we can use

  ```SQL
  SELECT * FROM table
  WHERE name like J%
  ```

  > so it will return all the 4 characters

- But what if we need only characters who have a name 4 letters long?
  For that we use "\_"

  Lets see how it works?

  ```SQL
  SELECT * FROM table
  WHERE name like J___
  ```

  > It will return only return "John" and "Jack". cause the rest are not 4 character long

---

```SQL
SELECT * FROM table
WHERE name like J%
```

> _This Query will only retrieve rows where first_name has initial J_.

### Use of "IN"

```SQL
SELECT * FROM employees
WHERE department IN ('HR','Finance','Admin');
```

> _This Query will only retrieve rows where department is one of the mentioned_.

### Use of "IS NULL"

```SQL
SELECT * FROM employees
WHERE phone_number IS NULL;
```

> _This Query will only retrieve rows where Phone_number is NULL_.

### Use of "AND", "OR", "NOT"

- These are called logical operators

  - "AND" : used to chain condition. Returns a output that satisfies all the conditions
  - "OR" : Returns a output where any one of the conditions are applied
  - "Not" : Returns a out[put where none of the conditions are satisfied]
