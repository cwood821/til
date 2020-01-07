# Discard untracked changes 

To discard untracked changes and revert changes to the head of the current branch: 

```
git clean -df
git checkout -- .
```

With git clean, `-d` will recurse into untracked directories.

See this [Stack Overflow post](https://stackoverflow.com/questions/52704/how-do-i-discard-unstaged-changes-in-git#answer-12184274).