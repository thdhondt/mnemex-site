---
title: "Symbols"
menutitle: "Symbols"
chapter: False
weight: 22
---

## Url

```url
https://mnemex.io/api/v1/symbols
```

## Input

| Parameter | Default | Description |
| --------- | ------- | ----------- |
| exchange  | -       | the name of the exchange platform |

## Result

| Field      | Default | Description |
| ---------- | ------- | ----------- |
| symbol     | string  | the name of the asset pair |
| base       | string  | the base currency |
| quote      | string  | the quote currency |
| symbolid   | string  | the exchange name of the asset pair |
| baseid     | string  | the exchange base currency |
| quoteid    | string  | the exchange quote currency |

## Examples

```url
https://mnemex.io/api/v1/symbols?exchange=binance
```
