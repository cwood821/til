# Filter a list with list comprehension

A compact way to filter a list in python is to use list comprehension: 

```python
some_filtered_list = [item for item in some_list if item.attribute == value]
```

Alternatively, a lambda function will work:

```python
some_filtered_list = filter(lambda item: item.attribute == value, some_list)
```

For discussion of performance and style, see this [StackOverflow post](https://stackoverflow.com/questions/3013449/list-comprehension-vs-lambda-filter).
