# Convert an integer to hex, octal, or binary

To convert an integer to a differently-based numeral system, pass the [radix](https://en.wikipedia.org/wiki/Radix) (base) to the `toString` method.

Example to convert `100` to binary:

```javascript
(100).toString(2) // 1100100
```

It works with other bases (8, 16, etc.). 

Convert back to base 10 with `parseInt`:

```javascript
parseInt("1100100", 2); // 100
```

See this [Stack overflow post](https://stackoverflow.com/questions/30954085/conversion-from-decimal-to-octal-binary-and-hexadecimal-in-javascript#30954162) for discussion.
