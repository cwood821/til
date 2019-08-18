# Print sorted disk usage across device

Print a list of disk usage across files and folders on a device, sorted by human readable size units, with:

```bash
du -hc 2>/dev/null | sort -h
```

Note: `2>/dev/null` will suppress permission denied errors. 

Hat tip to [this post](https://serverfault.com/questions/62411/how-can-i-sort-du-h-output-by-size).

