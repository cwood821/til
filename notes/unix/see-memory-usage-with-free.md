# See memory usage with free command


Output of the `free` command looks like:
```
              total        used        free      shared  buff/cache   available
Mem:        2038456     1049380       69136      140616      919940      705260
Swap:       1048572      283392      765180
```

## Columns
Mem

- total: RAM on computer
- used: Used memory `total-(free+buffers+cache)`
- free: Unnused memory
- shared: memory dedicated to `tmpfs` filesystems
- buff/cache: Memory used by buffers and cache
- available: Memory available to applications

Swap:

- total: size of swap file/partition
- used: swap space in use
- free: unnused swap space

Cache holds accessed files in RAM. If needed, these can be purged to reclaim the memory.

Swap is a file/partition on the hard disk where RAM contents may be copied to free up memory. See more [here](https://www.linux.com/news/all-about-linux-swap-space/).

Hat tip to [this post](https://www.howtogeek.com/456943/how-to-use-the-free-command-on-linux/).