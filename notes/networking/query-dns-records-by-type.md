# Query DNS records by type with dig

Query specific types of DNS records, like TXT or MX by specifiying them after the domain.

```sh
dig +nocmd google.com mx +noall +answer
```

See the man page for behavior of the `+...` options.

Hat tip [this post](https://linuxize.com/post/how-to-use-dig-command-to-query-dns-in-linux/).