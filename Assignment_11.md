# PostgreSQL Homework 11 

<br>

## Q1 First name columns in actor and customer tables:
```sql
    (SELECT first_name FROM actor)
    UNION
    (SELECT first_name FROM customer)
```

<br>

## Q2 Intersection of first name columns in actor and customer tables:
```sql
    (SELECT first_name FROM actor)
    INTERSECT
    (SELECT first_name FROM customer)
```

<br>

## Q3 First names that exists in actor table not not exist in customer table:
```sql
    (SELECT first_name FROM actor)
    EXCEPT
    (SELECT first_name FROM customer)
```

<br>

## Q4 First 3 questions but repeating values included:
```sql
    (SELECT first_name FROM actor)
    UNION ALL
    (SELECT first_name FROM customer);

    (SELECT first_name FROM actor)
    INTERSECT ALL
    (SELECT first_name FROM customer);

    (SELECT first_name FROM actor)
    EXCEPT ALL
    (SELECT first_name FROM customer);
```


<br><br>

---

The data that used for this assignment is sample data which obtained from 
[here](https://www.postgresqltutorial.com/postgresql-sample-database/)