# Do not paginate git output

Git usees a pager program by default. This is set in git config. If you want to not use the pager for a one-off command, use `--no-pager`:

```
git --no--pager log
```

Hat tip to [this post](https://stackoverflow.com/questions/2183900/how-do-i-prevent-git-diff-from-using-a-pager#2183920).