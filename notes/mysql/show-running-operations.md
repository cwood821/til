# Show running MySQL operations

To show a list of running operations on a MySQL server, use:

```mysql
SHOW FULL PROCESSLIST;
```

This will show you operations running on server threads, including information like time.

Kill a process with the `KILL <num>` query.

See [the documentation](https://dev.mysql.com/doc/refman/8.0/en/show-processlist.html).