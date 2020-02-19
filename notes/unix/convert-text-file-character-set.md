# Convert text file character set

Use the `iconv` utility to convert files between character sets.

```bash
iconv -c -t WINDOWS-1252 some-utf8-file.txt > some-file-with-windows-character-set.txt 
```

The `-c` option above discards characters that are not in the output characer set. 

List available sets with the `-l` option:
```
iconv -l
```

Read [the documentation](https://linux.die.net/man/1/iconv) for other options.

Hat tip to [this post](https://stackoverflow.com/questions/64860/best-way-to-convert-text-files-between-character-sets#64889).

