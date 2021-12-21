# PostgreSQL Homework 9 

<br>

## Q1 Cities from city table and countries from country table inner joined:
```sql
    SELECT city,country FROM city
    JOIN country ON city.country_id = country.country_id;
```

<br>

## Q2 First name and last name from customer table according to the customer ids from payment table:
```sql
    SELECT first_name,last_name,payment_id FROM payment
    JOIN customer ON payment.customer_id = customer.customer_id;
```

<br>

## Q3 Rental ID, first name and last name from customer table according to the customer ids from rental table:
```sql
    SELECT rental_id,first_name,last_name FROM rental
    JOIN customer ON customer.customer_id = rental.customer_id;
```


<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)