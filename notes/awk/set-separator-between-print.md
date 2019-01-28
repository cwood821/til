# Set separator between print statements in awk

To set the separator between print statements in awk, set the `ORS` variable:

```
awk 'BEGIN { ORS=" " }; {print $1; print $2; }'
```

This will separate both print statements by an empty space.

See this discussion on [Stack Overflow](https://stackoverflow.com/questions/24331687/is-it-possible-to-print-the-awk-output-in-the-same-line
). For more information, read the [awk man page](https://linux.die.net/man/1/awk).

