# Filter test run by title

To filter tests when running jest, add the `-t` option. 

```
jest -t 'title of test'
```

This will skip tests with titles that don't match. 

When running with `npm test`, remember the `--`to pass along the extra option.

```
npm test -- -t'title of test'
```

See this [StackOverflow post](https://stackoverflow.com/questions/42827054/how-do-i-run-a-single-test-using-jest#42897994).

