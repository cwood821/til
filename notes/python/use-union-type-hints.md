# Use union type hints in Python

Python 3.5+ allows optional type hints. To type hint a union (i.e. x or y), use the Union type:

```python
from typing import Union

def hello_or_nothing(msg: str) -> Union[str, None]:
  if msg == "hello":
    return "hello"
  else:
    return None

```

See [the documentation](https://docs.python.org/3/library/typing.html#typing.Union).

Note: there is an explicit [Optional type](https://docs.python.org/3/library/typing.html#typing.Optional) which is equivalent to `Union[x, None]`.