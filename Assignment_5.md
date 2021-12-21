# PostgreSQL Homework 5 

<br>

## Q1 5 Longest films where title ends with 'n' from film table:
```sql
    SELECT * FROM film
    WHERE title LIKE ('%n')
    ORDER BY length DESC
    LIMIT 5;
```

<br>

## Q2 Second 5 membered set of the shortest movies where title ends with 'n' from film table  :
```sql
    SELECT * FROM film
    WHERE title LIKE ('%n')
    ORDER BY length
    OFFSET 5
    LIMIT 5;
```

<br>

## Q3 First 4 datas where store id equals 1 and ordered by last name from customer table:
```sql
    SELECT * FROM customer
    WHERE store_id = 1
    ORDER BY last_name DESC
    LIMIT 4;
```


<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)
