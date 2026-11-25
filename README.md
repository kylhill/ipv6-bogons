# ipv6-bogons

## Purpose

A curated list of reserved and special-purpose IPv6 network ranges
for use in firewall address sets and traffic filtering.

## Getting started

Use `ipv6-bogons.txt` as input to an nftables set or other
firewall configuration generator.

Extract the CIDR entries without comments or blank lines:

```sh
grep -Ev '^[[:space:]]*(#|$)' ipv6-bogons.txt
```

Apply filtering according to the interface and network policy.
Some listed ranges are valid within local IPv6 networks.

## Documentation

- [IPv6 bogon ranges](ipv6-bogons.txt)
- [IANA IPv6 Address Space](https://www.iana.org/assignments/ipv6-address-space/)
- [IANA IPv6 Special-Purpose Address Registry](https://www.iana.org/assignments/iana-ipv6-special-registry/)
- [License](LICENSE)