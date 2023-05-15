# mzm'clash rules
``` yaml
rule-providers:
  telegram:
    type: http
    behavior: classic
    url: "https://raw.githubusercontent.com/mzmwd/clash-rules/main/telegram.txt"
    path: ./ruleset/telegram.yaml
    interval: 86400

  media:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/mzmwd/clash-rules/main/media.txt"
    path: ./ruleset/media.yaml
    interval: 86400

  youtube:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/mzmwd/clash-rules/main/custom.txt"
    path: ./ruleset/custom.yaml
    interval: 86400
```