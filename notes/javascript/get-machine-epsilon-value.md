# Get machine epsilon value in JavaScript

To find the [machine epsilon](https://en.wikipedia.org/wiki/Machine_epsilon) value for JavaScript, use `Number.EPSILON`. This is effectively the maximum possible rounding error for floating point numbers.

```javascript
// Number.EPSILON
Math.abs(0.2 - 0.3 + 0.1) < Number.EPSILON
// true
```

See [the docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/EPSILON).
