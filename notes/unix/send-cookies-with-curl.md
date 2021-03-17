# Send cookies with curl command 

To send cookies with the curl command, you can use `-b` or `--cookie`. The `-b` allows either a file name or a string with key value pairs.

```shell
curl -b "MY_TOKEN=VALUE" http://test.com
```

Hat tip to [this post](https://stackoverflow.com/questions/15995919/how-to-use-curl-to-send-cookies#15996114).