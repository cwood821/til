# Add a user to a group in Linux

To add a user to a group, use the `usermod` command:

```bash
usermod -aG <groupname> <username>
```

The `-a` option adds the user to the listed groups without removing them from groups they are already a part of and the `-G` option designates that the listed groups will be secondary groups, rather than primary.

See this [Stack Overflow post](https://askubuntu.com/questions/2214/how-do-i-add-a-user-to-the-sudo-group#2224) and [nixCraft](https://www.cyberciti.biz/faq/howto-linux-add-user-to-group/).

