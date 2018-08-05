# Sign git commits with GPG

You can sign your git commits with your GPG key. To do set it up, follow the Github [instructions](https://help.github.com/articles/signing-commits-using-gpg/). Taking this step improves the integrity of git commits.

1. [Generate a GPG Key](https://help.github.com/articles/generating-a-new-gpg-key/)
2. [Tell git about your GPG key](https://help.github.com/articles/telling-git-about-your-gpg-key/)
3. [Set git configuration to sign commits](https://help.github.com/articles/signing-commits-using-gpg/)

Sign your commits with the following flags:
```bash
git commit -S -m your commit message
```

On Mac, you may need to download the [GPG tools suite](https://gpgtools.org/). 