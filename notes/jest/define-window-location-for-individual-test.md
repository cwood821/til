# Define window.location.href for an individual test

To set the value of `window.location.href` for a single test in Jest, replace the window global object:

```javascript
global.window = Object.create(window);
Object.defineProperty(window, 'location', {
  value: {
    href: `https://my-test-url.com/some-path`
  },
  writable: true,
});
```

The writable property is important to be able to set this value again in a separate test within the same suite.

Note: This solution seems verison dependent. See [this discussion](https://github.com/jsdom/jsdom/issues/2112) on Github.
