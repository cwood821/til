# See differences between files with `diff` command

The diff command allows you to quickly compare differences between two files.

Usage:
```bash
diff example1.txt example2.txt
```

To see differences in context, use the `-c` flag. This produces differences similar to git, with pluses and minuses shown in context by new and deleted lines.

```
diff -c example1.txt example2.txt
```

To only check if two files differ without printing differences, use the `-q --brief` pair of flags.
```
diff -q --brief example1.txt example2.txt
```

This is regularly useful for checking updates and troubleshooting expected responses from services.

See the [man page](https://linux.die.net/man/1/diff) for more options.