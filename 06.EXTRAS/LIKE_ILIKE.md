## Difference

- LIKE --> Case Sensitive
- ILIKE --> Case Insensitive

## Syntax

- Syntax of LIKE command

```SQL
SELECT column_name(s)
FROM table_name
WHERE column_name LIKE pattern;
```

- Syntax of ILIKE command

```SQL
SELECT column_name(s)
FROM table_name
WHERE column_name ILIKE pattern;
```

## WILDCARD CHARACTERS

- "%" : Represents any sequence of characters
- "\_" : Represents a single character
- "[]" : Represents a character class, allowing you to match any single character within the specified set.

## Usage

- When searching for values with a certain pattern
- Comes in handy for partial searches
- To retrieve records that contain a specific substring
- Filtering data based on pattern

## USE of []

used for alternate words or spellings

### Example

```SQL
SELECT product_name
FROM products
WHERE product_name LIKE 'colo[u]r'
```
