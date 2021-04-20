# Return first non-null value from set with `COALESCE` function

To return the first non-null value from a set, use the `COALESCE` function:

```sql
SELECT 
    firstName, city, COALESCE(homeAddress, workAddress, 'N/A'), country
FROM
    employees;
```

Found in [this post](https://www.mysqltutorial.org/mysql-coalesce/).