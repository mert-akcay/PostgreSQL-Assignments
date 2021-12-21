# PostgreSQL Homework 4 

<br>

## Q1 Different values in replacement cost column from film table:
```sql
    SELECT DISTINCT replacement_cost FROM film;
```

<br>

## Q2 Nıumber of columns from the previous question:
```sql
    SELECT COUNT(DISTINCT replacement_cost) FROM film;
```

<br>

## Q3 Number of columns where title starts with 'T' and rating equals to 'G' from film table:
```sql
    SELECT COUNT(*) FROM film
    WHERE title LIKE ('T%') AND rating = ('G');

```

<br>

## Q4 Number of columns where country name has 5 characters from country table :
```sql
    SELECT COUNT(*) FROM country
    WHERE country LIKE ('_____');

```

<br>

## Q5 Number of columns where city name ends with insensitive 'r' from city table:
```sql
    SELECT COUNT(*) FROM city
    WHERE city ILIKE ('%r');

```

<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)
