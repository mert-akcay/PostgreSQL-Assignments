# PostgreSQL Homework 8 

<br>

## Q1 5 Update operation to the data obtained from Mockaroo:
```sql
    UPDATE employee
    SET name = 'Mert',
        birthday = '1945-05-10',
        email = 'mert@mail.com'
    WHERE id = 1;

    UPDATE employee
    SET id = 51,
        birthday = '1945-05-10',
        email = 'mert@mail.com'
    WHERE name = 'Valeria';

    UPDATE employee
    SET id = 52,
        name = 'Ahmet',
        email = 'ahmet@mail.com'
    WHERE birthday = '1956-03-15';

    UPDATE employee
    SET id = 53,
        name = 'Ahmet',
        birthday = '1956-03-15'
    WHERE email = 'ppowland15@cloudflare.com';

    UPDATE employee
    SET birthday = '1945-05-10',
        email = 'mert@mail.com'
    WHERE name LIKE ('B%');
```

<br>

## Q2 5 Delete operation to the data obtained from Mockaroo:
```sql
    DELETE FROM employee
    Where name = 'Mert';

    DELETE FROM employee
    Where birthday = '1968-08-04';

    DELETE FROM employee
    Where email = 'pmunghamw@state.tx.us';

    DELETE FROM employee
    Where id = 10;

    DELETE FROM employee
    Where name LIKE ('%a');
```




