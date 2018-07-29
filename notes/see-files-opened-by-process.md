# See list of files opened by a process

To see a list of files currently open by processes, you can use the [`lsof`](https://en.wikipedia.org/wiki/Lsof) command. Pair with a flag or `grep` for more power.

To see all the files Firefox has open, for example:
```bash
lsof | grep firefox
```

To see processes using a file on a specific port number, use the `-i` flag.
```bash
lsof -i :3000 
```

This should return a result like:
```bash
COMMAND   PID          USER   FD   TYPE             DEVICE SIZE/OFF NODE NAME
node    16150 christianwood   13u  IPv6 0x7cbe288dc6d3a25f      0t0  TCP *:hbci (LISTEN)
```

See the [man page](https://linux.die.net/man/8/lsof) for full list of options.

## Using lsof to troubleshoot port conflicts in local development
Say you want to spin up a local development server, but you receive an error that the port you want to use is already in use.

With node, the error might look like this for a develpment server running on port 3000: ```Error: listen EADDRINUSE :::3000```.

Track down what process is using that port with `lsof`:
```bash
lsof -i :3000
```
Get the ID of the offending process:
```bash
COMMAND   PID          USER   FD   TYPE             DEVICE SIZE/OFF NODE NAME
node    16150 christianwood   13u  IPv6 0x7cbe288dc6d3a25f      0t0  TCP *:hbci (LISTEN)
```
Kill that process to free up the port:
```bash
kill 16150
```