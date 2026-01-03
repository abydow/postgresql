## Structure of challenges

1. Business Situation
2. Expected Results
3. Hints
4. Solution

## Challenge 1

### Business Situation

You are running a DVD rental store and want to find titles of films released in or after the year 2000 that have rating of 'PG-13'.You also need to know the replacement cost of these films.

### Expected Results

"Bright Encounters" 12.99
"Airplane Sierra" 28.99
"Alabama Devil" 21.99
"Alter Victory" 27.99
"Anthem Luke" 16.99
"Apollo Teen" 15.99
"Arachnophobia Rollercoaster" 24.99
"Argonauts Town" 12.99
"Attacks Hate" 21.99
"Attraction Newton" 14.99

### Hints

- Filter based on their release year and rating
- Rating column stores the film's rating
- release_year column stores the year a film was released

### Solution

```SQL
SELECT title,replacement_cost FROM film
WHERE release_year >= 2000 AND rating = 'PG-13';
```

> _IMP. news_ : _"" and '' are different in postgreSQL, so if you put "PG-13" there it will not work_

## Challenge 2

### Business Situation

You want to see the titles of films with a rating of 'PG' and replacement cost of $10.99

### Expected Results

"Cowboy Doom"
"Gaslight Crusade"
"Kentuckian Giant"
"Mile Mulan"
"Secretary Rouge"
"Stock Glass"
"Super Wyoming"
"Tootsie Pilot"

### Hints

- You need to filter films based on their rating and replacement cost
- The rating column stored the film's rating
- The replacement_cost column represents the cost to replace a film

### Solution

```SQL
SELECT title FROM film
WHERE replacement_cost = 10.99 AND rating = 'PG';
```

## Challenge 3

### Business Situation

Find the titles of films released either before the year 2000 or with a replacement cost less than 10$

### Expected Results

"Anaconda Confessions"
"Cider Desire"
"Control Anthem"
"Daisy Menagerie"
"Deliverance Mulholland"
"Dude Blindness"
"Edge Kissing"
"Encino Elf"
"Factory Dragon"
"Fellowship Autumn"

### Hint

- Filter based on release year and replacement cost
- Release year column stores the year of release
- Replacement cost column represents the cost to replace a film

### Solution

```SQL
SELECT title FROM film
WHERE replacement_cost < 10 OR release_year < 2000;
``
```
