# Dump database without locking 

By default, `mysqldump` will lock tables while dumping them. This can be desirable in some cases. In other cases, use ``--single-transaction` and `--skip-lock-tables` to run the dump as a single, non-locking transaction. 

```
mysqldump --single-transaction --skip-lock-tables some_db > some_db.sql
```

See the [documentation](https://dev.mysql.com/doc/refman/8.0/en/mysqldump.html#option_mysqldump_lock-tables) and read more [here](https://serversforhackers.com/c/mysqldump-with-modern-mysql).
