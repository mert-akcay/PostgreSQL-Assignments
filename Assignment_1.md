# PostgreSQL Homework 1 

<br>

## Q1 : Title and description columns from films table:
```sql
    SELECT title,description FROM film;
```

<br>

## Q2 All Columns where length between 60 and 75 from films table:
```sql
    SELECT * FROM film
    WHERE length>60 AND length<75;
```

<br>

## Q3 All Columns where rental rate equals 0.99 and replacement cost equals 12.99 or 28.99 from films table:
```sql
    SELECT * FROM film
    WHERE rental_rate=0.99 AND (replacement_cost = 12.99 OR replacement_cost = 29.99);
```

<br>

## Q4 Last name of the customer Mary from the customer table:
```sql
    SELECT last_name FROM customer
    WHERE first_name = 'Mary';
```

<br>

## Q5 All columns where length is not greater than 50 and rental rate is not 2.99 or 4.99 from films table:
```sql
    SELECT * FROM film
    WHERE NOT length > 50 AND (rental_rate=2.99 OR rental_rate = 4.99);
```

<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)
