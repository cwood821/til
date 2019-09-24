# Run cleanup function with `useEffect`

Similar to the class lifecycle method `componentWillUnmount`, the `useEffect` allows running a function to clean up. To do so, return a cleanup function from the `useEffect` function parameter.

```react
useEffect(() => {
  return () => {
    // Clean up stuff 
  };
});
```

See [the docs](https://reactjs.org/docs/hooks-reference.html#cleaning-up-an-effect).