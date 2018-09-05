# Remove stale remote tracking branches

If someone deletes a remote branch and you still have a local tracking branch, the local tracking branch will not be removed by default with `fetch`. You can add the `--prune` flag to delete it.

```
git fetch --prune
```

You can also use the prune command with remote:

```
git remote prune origin
```

To see the list of your remote tracking branches, use:

```
git branch -r
```

For more detail on distinctions, read this [Stack Overflow post](https://stackoverflow.com/questions/20106712/what-are-the-differences-between-git-remote-prune-git-prune-git-fetch-prune#20107184).