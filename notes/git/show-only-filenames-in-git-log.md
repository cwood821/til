# Show only filenames in git log output

To see only the names of files that changed with git log, use the `--name-only` flag.

```bash
git log --name-only 
```
To show name and status (modified, added, etc.) of the files, use `--name-status`
```bash
--name-status
```

Tacking on `--oneline` makes both options less verbose.

Found on [Stack Overflow](https://stackoverflow.com/questions/14207414/how-to-show-changed-file-name-only-with-git-log). Read the [git log documentation](https://www.git-scm.com/docs/git-log) for more options.
