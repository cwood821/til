# Dump database to archive 

To save a mongodb database to an archive, use the `mongodump` tool with the `archive` and `gzip` flags. 

```
mongodump --db my_db --gzip --archive > my_db.gz
```

See [documentation mongodump](https://docs.mongodb.com/manual/reference/program/mongodump/). 


