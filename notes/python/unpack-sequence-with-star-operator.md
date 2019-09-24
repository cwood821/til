# Unpack sequences and lists with star operator

Unpack a sequence or collection into positional arguments with the star operator:

```python
def multiply(first, second):
    return first + second

nums = (1, 2)

s = multiply(*nums)
```

Hat tip to [this post](https://stackoverflow.com/questions/2921847/what-does-the-star-operator-mean#answer-2921893). See [the documentation](https://docs.python.org/3/tutorial/controlflow.html#unpacking-argument-lists).
