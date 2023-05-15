# mzm'clash rules
``` yaml
rule-providers:
  telegram:
    type: http
    behavior: classic
    url: "https://raw.githubusercontent.com/mzmwd/clash-rules/main/telegram.yaml"
    path: ./ruleset/telegram.yaml
    interval: 86400

  media:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/mzmwd/clash-rules/main/media.yaml"
    path: ./ruleset/media.yaml
    interval: 86400

  youtube:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/mzmwd/clash-rules/main/custom.yaml"
    path: ./ruleset/custom.yaml
    interval: 86400
```
```
rules:
  - RULE-SET,media,Media
  - RULE-SET,telegram,Media
  - RULE-SET,custom,Proxy
  - GEOIP,CN,DIRECT
  - MATCH,PROXY
```
