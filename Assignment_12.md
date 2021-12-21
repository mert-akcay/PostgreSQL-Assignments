# PostgreSQL Homework 12

<br>

## Q1 Amount of films which has a length greater than average length from film table:
```sql
    SELECT COUNT(*) FROM film
    WHERE length > (SELECT AVG(length) FROM film);
```

<br>

## Q2 Amount of film which has max rental rate value from film table:
```sql
    SELECT COUNT(*) FROM film
    WHERE rental_rate = (SELECT MAX(rental_rate) FROM film);
```

<br>

## Q3 Film which has minimum rental rate and minimum replacement values from film table:
```sql
    SELECT * FROM film
    WHERE rental_rate = (SELECT MIN(rental_rate) FROM film) 
    AND replacement_cost = (SELECT MIN(replacement_cost) FROM film);
```

<br>

## Q4 The most active customer from customer table:
```sql
    SELECT * FROM customer
    WHERE customer_id = (
        SELECT customer_id FROM payment
        GROUP BY customer_id
        ORDER BY COUNT(*) DESC
        LIMIT 1
    );
```


<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)