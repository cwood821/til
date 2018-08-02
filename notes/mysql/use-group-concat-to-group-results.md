# Use `group_concat` in MySQL to concatenate group results into a single string

Group concat concatenates strings from a group into a single string. 

Say you have node to tag relationship of many to many and you want to return a result where one column lists all the tags associated with a node as a comma-separated list.

```sql
SELECT DISTINCT node.title, group_concat(taxonomy_term_data.name separator ', ') AS tags
FROM node
INNER JOIN taxonomy_index
ON taxonomy_index.nid = node.nid
INNER JOIN taxonomy_term_data
ON taxonomy_index.tid = taxonomy_term_data.tid
GROUP BY node.nid
```

The output will be in this format:
```
title, tags
'First node title', 'First taxonoy term name, Second taxonomy term name'
```

[Official Documentation](https://dev.mysql.com/doc/refman/5.5/en/group-by-functions.html#function_group-concat), [Stackoverflow post](https://stackoverflow.com/questions/13451605/how-to-use-group-concat-in-a-concat-in-mysql#13451984)
