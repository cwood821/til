# Mark releases with tags

Tags let you note certain points in history, typically to mark a version release.

To create an annotated tag:

```
git tag -a v1.1 -m"Version 1.0"
```


To list tags (the `-n` will include annotations):

```
git tag -l -n 
```

To show differences between releases, you can use git diff and reference a tag:

```
git diff v1.0..v1.1
```

Delete a tag with `-d`:

```
git tag -d name-of-tag
```

## Tags are not pushed to remotes by default

You must push tags explicitely to share them.

```
git push origin tag-name
```


## Checkout tags into a new branch
Tags just identify commits. They can be checked out, but you should create a new branch on the tag. Otherwise you end up in detached head state and your new commits will be orphaned.

So: 

```
git checkout -b v0.1
```

Full [documentation here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
