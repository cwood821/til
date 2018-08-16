# Check disk usage with `du` command

Find files that are eating up hard drive space with the du command.

To check the memory usage of directories, use du:
```bash
du -h my-project-dir
```
This prints the disk usage of both my-project-dir and each subdirectory. The -h prints results in 'human readable' format (i.e. Kilobytes, Megabytes, etc.)

### Other flags
- -a Flag will print all files and directories
- -c Provides a grand total usage on the last line
- -s Summarize each result (only display total for each argument)

## Exclude certain files from the listing
Use --exclude to not show files that match a pattern.

```bash
du -ah --exclude="*.txt" my-project-dir 
```

## See size that would be transferred over a network

Use --apparent-size to see the apparent file size, rather than disk usage. This is useful for estimating the size that would be transferred over a network.
```
du -sh --apparent-size /path/to/directory
```

See the [man page](https://linux.die.net/man/1/du) for more details. 