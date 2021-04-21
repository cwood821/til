# Make an array of files from glob pattern


```shell
myarr=(~/somedir/*)
```

Combine with `shopt -s nullglob` to handle no matching files. Reference the [bash manual](http://www.gnu.org/savannah-checkouts/gnu/bash/manual/bash.html#Conditional-Constructs), which says:

> If set, Bash allows filename patterns which match no files to expand to a null string, rather than themselves.


See [this stack overflow post](https://stackoverflow.com/questions/21668471/bash-script-create-array-of-all-files-in-a-directory#21668536).