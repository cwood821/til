# Forward SSH Agent with connection with `-A` flag

Forwarding your SSH agent will allow you to connect from a remote machine to a third machine with your SSH agent. The agent allows you to connect without storing private keys on the intermediate machine. The agent will connect back to your local machine to validate your keys.

Use the `-A` flag to forward ssh agent.
```
ssh some-host.com -A
```

To test if the agent is running, you can list out private keys associated with it:
```
ssh-add -l
```

See this [deep dive](http://www.unixwiz.net/techtips/ssh-agent-forwarding.html). For a discussion of security implications, see [this link](https://yakking.branchable.com/posts/ssh-A/). 

