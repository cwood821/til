# Use clamp to control values over a range

The clamp function in css maintains a value within an upper and lower bound with preference for a middle value.

```css
// min, value, max
width: clamp(100px, 50%, 400px);
```

Resolves as `max(MIN, min(VAL, MAX))`.

Read more on [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp()).