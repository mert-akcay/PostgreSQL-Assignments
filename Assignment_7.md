# PostgreSQL Homework 7 

<br>

## Q1 Amount of films according to the rating from film table:
```sql
    SELECT rating, COUNT(*) FROM film
    GROUP BY rating;
```

<br>

## Q2 Amount of films according to the replacement cost which has greater than 50 from film table:
```sql
    SELECT replacement_cost, COUNT(*) FROM film
    GROUP BY replacement_cost
    HAVING COUNT(*)>50;
```

<br>

## Q3 Number of customers according to the store id from customer table:
```sql
    SELECT store_id, COUNT(*) FROM customer
    GROUP BY store_id;
```

<br>

## Q4 Country ID and city amount of the according to the max city amount from city table:
```sql
    SELECT country_id ,COUNT(*) FROM city
    GROUP BY country_id
    ORDER BY COUNT(*) DESC
    LIMIT 1;
```


<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)
