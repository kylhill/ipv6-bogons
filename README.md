# ipv6-bogons
IPv6 Bogon Ranges suitible for generating set filters to use in nftables

## Generated from:
* 'whois -h whois.ripe.net fltr-martian-v6'
  - Teredo (2001::/32) and 6to4 (2002::/16) addresses are NOT FILTERED to avoid dropping legitimate traffic
* "IPv6 Additional Bogon Ranges" from https://ipgeolocation.io/resources/bogon.html
  - Teredo (2001::/32) and 6to4 (2002::/16) IPv4-mapped Bogons
