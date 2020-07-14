# Extract substrings from variables

Extract substrings from BASH variables: 

```bash
MY_STRING="hello"
SUB_STR=${MY_STRING:0:2}

echo $SUB_STR 
# he
```

See [this post](https://unix.stackexchange.com/questions/303960/index-a-string-in-bash).