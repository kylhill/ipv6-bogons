# ipv6-bogons
IPv6 Bogon Ranges suitible for generating ipset filters to use in ip6tables

## Generated from:
* 'whois -h whois.ripe.net fltr-martian-v6'
  - RFC 4291 IETF Reserved addresses are NOT FILTERED to reduce future maintenance needs
  - Teredo (2001::/32) and 6to4 (2002::/16) addresses are NOT FILTERED to avoid dropping legitimate traffic
  - fe80::/10 is NOT FILTERED to allow link-local communication to function
* "IPv6 Additional Bogon Ranges" from https://ipgeolocation.io/resources/bogon.html
  - Teredo (2001::/32) and 6to4 (2002::/16) IPv4-mapped Bogons
