## Revert file to some previous commit

To revert a file in git to some previous commit, just check out the individual file at the hash of that commit:

```
git checkout c5f567 -- file1/to/revert 
```

[Hat tip](https://stackoverflow.com/questions/215718/how-can-i-reset-or-revert-a-file-to-a-specific-revision)