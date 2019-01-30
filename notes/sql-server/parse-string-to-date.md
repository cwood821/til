# Parse string to date in SQl Server/MSSQL

If you have a string that must be converted to a date to accomdate comparisons, use the `PARSE` function:

```
PARSE('31 December 2017' AS date USING 'en-US')
```

See the [documentation](https://docs.microsoft.com/en-us/sql/t-sql/functions/parse-transact-sql?view=sql-server-2017).
