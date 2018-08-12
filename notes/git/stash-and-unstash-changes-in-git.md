# Stash and unstash changes in git

To stash changes that have not yet been committed, use git stash:

```
git stash
```

Stashing adds staged and unstaged changes to a list. To see the list of stashes:

```
git stash list
```

## Re-applying (unstashing) changes

To apply a stash to the current branch and keep it in the stash list, use apply:

```
git stash apply
```

To apply a stash to the current branch and remove it from the stash list, use pop:
```
git stash pop
```

By default, both `apply` and `pop` will apply the most recent stash. To apply a specific stash, use its identifier:

```
git stash apply stash@{0}
```


## Remove stashes
```
git stash drop stash@{1}
```

For more information, see [Git stash tutorial](https://www.atlassian.com/git/tutorials/saving-changes/git-stash) from Atlassian and the [Git scm](https://www.git-scm.com/docs/git-stash) documentation.

