# Extend behavior of Python functions with decorators

To extend the behavior of a Python function without changing its implementation, you can decorate it.

The pattern looks like this:
```python
def some_decorator(func):
    def wrapper():
        print("Run before the function")
        func()
    return wrapper

def say_hello():
    print("Hello")

say_hello = some_decorator(say_hello)

say_hello()
# Will print:
# Run before the function 
# Hello
```

Python provides syntactic sugar with the `@` syntax:
```python
def some_decorator(func):
    def wrapper():
        print("Run before the function")
        func()
    return wrapper

@some_decorator
def say_hello():
    print("Hello")

say_hello()
# Will print:
# Run before the function 
# Hello
```

The decorator pattern takes advantage of functions being first-class citizens in Python. This pattern is useful to modify function behavior without changing existing implementation. It's also a useful method for checking cached values, authentication tokens in web requests, etc. Read more on [Code Ship](https://www.thecodeship.com/patterns/guide-to-python-function-decorators/) and [Real Python](https://realpython.com/primer-on-python-decorators/)