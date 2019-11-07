# Get PID of shell running script

To get the process id of the shell instance running a Bash script, use `$$`.

```shell
echo $$
```

From [the manual](http://www.gnu.org/savannah-checkouts/gnu/bash/manual/bash.html#index-_0024_0024):

> ($$) Expands to the process ID of the shell. In a () subshell, it expands to the process ID of the invoking shell, not the subshell.

There is also a BASHPID variable, but note the [differences in behavior in subshells](https://stackoverflow.com/questions/2493642/how-does-a-linux-unix-bash-script-know-its-own-pid#answer-2493659).

