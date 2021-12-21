# PostgreSQL Homework 10 

<br>

## Q1 Cities from city table and countries from country table left joined:
```sql
    SELECT city,country FROM city
    LEFT JOIN country ON city.country_id = country.country_id;
```

<br>

## Q2 First name and last name from customer table according to the customer ids from payment table:
```sql
    SELECT payment_id,first_name,last_name FROM customer
    RIGHT JOIN payment ON customer.customer_id = payment.customer_id;
```

<br>

## Q3 Rental ID, first name and last name from customer table according to the customer ids from rental table:
```sql
    SELECT rental_id,first_name,last_name FROM customer
    FULL JOIN rental ON customer.customer_id = rental.customer_id;
```


<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)