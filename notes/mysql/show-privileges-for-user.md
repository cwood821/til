# Show privileges for MySQL user

```sql
SHOW GRANTS FOR 'someuser'@'localhost';
```

You can show grants for the current user with:

```sql
SHOW GRANTS FOR CURRENT_USER;
```

See [official documentation](https://dev.mysql.com/doc/refman/8.0/en/show-grants.html). Hat tip to this [Server Fault post](https://serverfault.com/questions/117525/how-can-i-show-users-privileges-in-mysql).
