# Get fingerprint of ssh key

To get the fingerprint of an ssh key, run ssh-keygen with the following options:

SHA256

```sh
ssh-keygen -lf ~/.ssh/id_rsa.pub
```

MD5 (Github)

```sh
ssh-keygen -E md5 -lf id_rsa.pub
```

Hat tip to [this post](https://stackoverflow.com/questions/9607295/calculate-rsa-key-fingerprint).