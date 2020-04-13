# Handle signals with callback in NodeJS

Handle POSIX signals in NodeJS:

```javascript
process.on('SIGUSR2', function() {
  console.log("caught signal"); 
});
```

The above example uses `SIGUSR2`, which you can send from the terminal with:

```
kill -s SIGUSR2 pid-of-node
```

See a list of [POSIX signals](https://en.wikipedia.org/wiki/Signal_(IPC)).