# Get index of character in string

Awk string functions operate on characters. To find the index of a character in a string, use `index`:

```bash
echo "test" | awk '{print index($0, "s")}'
# 3
```

This will return the integer location of the first occurence of the search string or zero if it is not found.

See [String Functions](https://www.gnu.org/software/gawk/manual/html_node/String-Functions.html#String-Functions) in the manual. 