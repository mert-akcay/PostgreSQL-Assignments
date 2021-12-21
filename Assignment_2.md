# PostgreSQL Homework 2 

<br>

## Q1 All columns where replacement cost between 12.99 and 16.99 from film table:
```sql
    SELECT * FROM film
    WHERE replacement_cost BETWEEN 12.99 AND 16.99;
```

<br>

## Q2 First name and last name Columns where first name is Penelope or Nick or Ed from actor table:
```sql
    SELECT first_name,last_name FROM actor
    WHERE first_name IN ('Penelope','Nick','Ed');
```

<br>

## Q3 All Columns where rental rate equals 0.99 or 2.99 or 4.99 and replacement cost equals 12.99 or 15.99 or 28.99 from film table:
```sql
    SELECT * FROM film
    WHERE (rental_rate IN (0.99,2.99,4.99)) AND (replacement_cost IN (12.99,15.99,28.99));

```


<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)
