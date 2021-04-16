# Execute multiple commands with xargs

To execute multiple commands in sequence with xargs, while using the piped data, use string replacement with the `-I` flag:

```
find mydir -type d -maxdepth 1 -not -name 'mydir' | xargs -I % sh -c 'cd % && npm run build'
```

This find every directory under `mydir` except itself, change directory into it, then run `npm run build`. 