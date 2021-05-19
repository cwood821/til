# Add unit at end of calc expression

If you have an expression in calc, but want to delay adding the unit until the very end, multiply by 1 of the unit last:

```css
padding: calc((2 * 4 / 2) * 1rem);
```


This will resolve the expression to the multiplied unit.

Hat tip to [this post](https://css-tricks.com/a-complete-guide-to-calc-in-css/).