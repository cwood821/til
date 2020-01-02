# Perform case-sensitive string comparison with `BINARY` 

By default, MySQL string comparison is case-insensitive. To force case-sensitive comparison, use `BINARY`:

```sql
select * from my_posts where BINARY post_title = 'Test post';
```

This will only select posts with exactly 'Test post' as the title, not 'test post' or other variations. See [the documentation](https://dev.mysql.com/doc/refman/8.0/en/cast-functions.html#operator_binary).
