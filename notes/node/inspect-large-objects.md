# Inspect large objects 

Inspect large objects in Node when debugging:

```javascript
const util = require('util')

console.log(util.inspect(largeObject, {showHidden: false, depth: null}))
```

Hat tip to [Stack Overflow](https://stackoverflow.com/questions/10729276/how-can-i-get-the-full-object-in-node-jss-console-log-rather-than-object). See the [docs](https://nodejs.org/api/util.html#util_util_inspect_object_options).
