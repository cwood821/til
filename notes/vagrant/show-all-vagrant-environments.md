# Show all Vagrant environments

To see a list of vagrant environments on your machine:

```bash
vagrant global-status
```

This command loads a list from cache. To prune invalid entries, run the command with the `--prune` flag.

```bash
vagrant global-status --prune
```
[Official documentation](https://www.vagrantup.com/docs/cli/global-status.html) for the global-status command.

Alternately, if Vagrant uses Virtualbox, you can see all virtual machines running with the virtual box command line tool:

```bash
VBoxManage list runningvms
```
