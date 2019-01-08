# Hash values in SQL Server 

The [HASHBYTES](https://docs.microsoft.com/en-us/sql/t-sql/functions/hashbytes-transact-sql?view=sql-server-2017) function allows you to choose an algorithm and hash a value. Its ouput is binary.

You can use [SHA256](https://stackoverflow.com/questions/5335734/sha256-function-in-sql-server) (and others). 
For added security, [add a random, unique salt for each hash](https://www.mssqltips.com/sqlservertip/3293/add-a-salt-with-the-sql-server-hashbytes-function/).

Store them in a [binary column](https://stackoverflow.com/questions/14722305/what-kind-of-datatype-should-one-use-to-store-hashes), or Base64 encode them and store them as [VARCHAR(65)](https://stackoverflow.com/questions/2240973/how-long-is-the-sha256-hash).

Example, converting the hash:
```sql
CONVERT(VARCHAR(65), HASHBYTES('SHA2_256', CONCAT('SOME VALUE TO HASH', 'my_weak_salt')), 2)
```

