# Check file mime type with `file` command

To check a file's mime type from the shell, use the `file` command with the `--mime-type` flag:
```bash
file --mime-type the-file.png
```

Should output something like:
```bash
the-file.png: image/png
```

For alternative examples, see this [Stack Overflow post](https://stackoverflow.com/questions/2227182/how-can-i-find-out-a-files-mime-type-content-type#2227201).

### How it matches files
Underneath, the file command uses a database, typically located somewhere like `/usr/share/file/magic` to match files to types based on leading bytes of a file. 
For alternative locations, see [this Unix StackExchange post](https://unix.stackexchange.com/questions/151414/file-command-database-and-identifying-text-files#151420) or the [man page](https://linux.die.net/man/1/file) for the file command. For more information on the file specification, see [Wikipedia](https://en.wikipedia.org/wiki/File_%28command%29#Specification).