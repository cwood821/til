# Search historical commit diffs 

To lookup commits whose diff matches a regular expression, use the `-G` flag with `git log`.
```
git log -G "myRegex"
```

You can use other flags, also, to format the results. Notably, `-p` will show you the diff.

See the official documentation for the [`G` flag](https://git-scm.com/docs/git-log#Documentation/git-log.txt--Gltregexgt).
