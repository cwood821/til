# Test headers with curl

To test request headers, `curl` with the `-I` flag. That will return just the headers of the request.

```
curl -I https://christianwood.net
```
In case the response is a redirect, use the `L` flag to instruct curl to follow redirects. Hat tip to [David Walsh](https://davidwalsh.name/curl-follow-redirects).
