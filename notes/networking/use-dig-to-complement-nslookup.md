# Use `dig` to query DNS information as a complement to nslookup

The dig command queries DNS servers and responds with record information about a particular domain.

```bash
dig christianwood.net
```
Outputs:

```
; <<>> DiG 9.10.6 <<>> christianwood.net
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 33235
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;christianwood.net.		IN	A

;; ANSWER SECTION:
christianwood.net.	14399	IN	A	208.113.221.186
```

The answer section includes domain, [time to live](https://en.wikipedia.org/wiki/Time_to_live), and record information (in the above example, an A record pointing to 208.113.221.186).

In contrast to `nslookup`, dig will use the operating system's default Domain Name System resolver.

Read a breakdown of the output [here](https://ns1.com/blog/decoding-dig-output), or read the [man page](https://linux.die.net/man/1/dig).