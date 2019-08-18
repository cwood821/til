# Hide untracked files in git status

To hide untracked files in git status, use:

```bash
git status --untracked-files=no
```

The shorthand is:
```bash
git status -uno
```

This variation is useful for getting a clean view of changes when built files are polluting git status.