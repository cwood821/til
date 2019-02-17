# List indices on ElasticSearch cluster

To list which indices exist on a cluster, use the `_cat` api: 

```
curl http://localhost:9200/_cat/indices?v
```

Hat tip to [Coding Explained](https://codingexplained.com/coding/elasticsearch/listing-all-indexes-in-elasticsearch-cluster). Read [the documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/cat-indices.html).
