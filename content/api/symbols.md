---
title: "Symbols"
menutitle: "Symbols"
chapter: False
weight: 22
---

## Information

This method makes it possible to retrieve the symbols that are supported by the api. Any symbol is an asset pair with a base and quote currency. Consider for instance the symbol or asset pair ETH/BTC. The quote currency is ETH and the base currency is BTC. 

Note that this method returns also the symbol id, base id and quote id. 
CCXT has indeed standardize the asset pairs name, and we follow this standard. 
However, you might be interested to have the base and quote currency as they are list on their exchange. 

## Url

```url
https://mnemex.io/api/v1/symbols
```

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
