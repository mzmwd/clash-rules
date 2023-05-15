# mzm'clash rules
``` yaml
rule-providers:
  telegramcidr:
    type: http
    behavior: classic
    url: "https://raw.githubusercontent.com/mzmwd/clash-rules/release/telegram.txt"
    path: ./ruleset/telegram.yaml
    interval: 86400
```