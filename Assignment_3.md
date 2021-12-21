# PostgreSQL Homework 3 

<br>

## Q1 All columns where country name starts with 'A' and ends with 'a' from country table:
```sql
    SELECT * FROM country
    WHERE country LIKE ('A%a');
```

<br>

## Q2 All columns where country name has minimum 6 characters and ends with 'n' from country table:
```sql
    SELECT * FROM country
    WHERE country LIKE ('_____%n');
```

<br>

## Q3 All columns where country name has minimum 4 case insensitive 't' letter from country table:
```sql
    SELECT * FROM country
    WHERE country ILIKE ('%t%t%t%t%');

```

## Q4 All columns where title starts with 'C' letter and length greater than 90 and rental rate equals 2.99 from film table:
```sql
    SELECT * FROM film
    WHERE title LIKE ('C%') AND length>90 AND rental_rate=2.99;
```

<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)
