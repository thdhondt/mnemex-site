---
title: "Symbols"
menutitle: "Symbols"
chapter: False
weight: 22
---

## Information

URL: https://mnemex.io/api/v1/symbols

## Input

| parameters | Default | Description |
| ---------- | ------- | ----------- |
| exchange   | -       | the name of the exchange platform |

## Result

| parameters | Default | Description |
| ---------- | ------- | ----------- |
| symbol     | string  | the name of the asset pair |
| base       | string  | the base currency |
| quote      | string  | the quote currency |
| symbolid   | string  | the exchange name of the asset pair |
| baseid     | string  | the exchange base currency |
| quoteid    | string  | the exchange quote currency |

## Examples

```bash
curl https://mnemex.io/api/v1/symbols?exchange=binance
```
