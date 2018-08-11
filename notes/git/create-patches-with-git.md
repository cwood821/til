# Create patches with Git

To create a patch in git, first checkout a branch that has your desired changes.
```
git checkout my-patch-branch
```

Assuming that there are commited changes on this branch, run a git diff against the unpatched branch and output the result to a file:
```
git diff master > my-great-patch.patch
```

This is the recommended method for [Drupal patch submissions](https://www.drupal.org/node/707484). 

### Apply patches
Use git apply or git am to apply your patch.
```
git checkout master
git apply my-great-patch.patch
```

The [`am`](https://git-scm.com/docs/git-am) command will apply the patch as a commit, [`apply`](https://git-scm.com/docs/git-apply) will only make the changes.


### Format-patch command
An alternative to the diff method is to use the [format-patch](https://git-scm.com/docs/git-format-patch) command. This formats a patch and includes email information. See [this blog](https://www.devroom.io/2009/10/26/how-to-create-and-apply-a-patch-with-git/) for details.
