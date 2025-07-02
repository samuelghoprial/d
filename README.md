[General]
bypass-system = true
skip-proxy = 192.168.0.0/16,10.0.0.0/8
dns-server = 8.8.8.8

[Rule]
DOMAIN-SUFFIX,ubereats.com,PROXY
DOMAIN-KEYWORD,ubereats,PROXY
DOMAIN-SUFFIX,instacart.com,PROXY
DOMAIN-KEYWORD,instacart,PROXY
DOMAIN-SUFFIX,chipotle.com,PROXY
DOMAIN-KEYWORD,chipotle,PROXY

# Let Apple services bypass proxy
DOMAIN-SUFFIX,apple.com,DIRECT
DOMAIN-SUFFIX,icloud.com,DIRECT
DOMAIN-SUFFIX,me.com,DIRECT
DOMAIN-SUFFIX,pay.apple.com,DIRECT
DOMAIN-SUFFIX,itunes.apple.com,DIRECT

# Everything else stays on real IP
FINAL,DIRECT
