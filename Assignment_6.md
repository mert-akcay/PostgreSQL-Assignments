# PostgreSQL Homework 6 

<br>

## Q1 Average value of rental rates from film table:
```sql
    SELECT ROUND(AVG(rental_rate) , 3)  FROM film;
```

<br>

## Q2 Number of the datas where title starts with 'C' from film table:
```sql
    SELECT COUNT(*)  FROM film
    WHERE title LIKE ('C%');
```

<br>

## Q3 Max length of the film which has a rental rate value 0.99 from film table:
```sql
    SELECT MAX(length)  FROM film
    WHERE rental_rate = 0.99;
```

<br>

## Q4 Number of the datas which has unique replacement cost values and a length that greater than 150 from film table:
```sql
    SELECT COUNT(DISTINCT replacement_cost)  FROM film
    WHERE length > 150;
```


<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)
