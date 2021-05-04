# Detect Invalid Date Objects

If the JavaScript Date constructor fails to parse a date string, it will return an invalid Date object.

Even though it is invalid, it will still pass an `instanceof` check
``` js
let invalid = new Date("");
invalid instanceof Date // true
```

The `isNaN` function will return true for invalid dates and false for valid ones:
```js
isNaN(invalid) // true
```

There is some nuance when working across frame boundaries. See [this post](https://stackoverflow.com/questions/1353684/detecting-an-invalid-date-date-instance-in-javascript#1353711).