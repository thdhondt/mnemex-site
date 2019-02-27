---
title: "Trades"
menutitle: "Trades"
chapter: false
weight: 23
---

## Information

URL: https://mnemex.io/api/v1/trades

Hello world !!!

hihaaa

## Input

| parameters | default | description |
| ---------- | ------- | ----------- |
| exchange   | -       | the name of the exchange platform |
| symbol     | -       | the name of the asset pair |
| last       | 1000    | the last number of samples to etrieve |
| since      | now     | last timestamp to retrieve the data from |

## Result

| name  | type    | description           |
| ----- | ------- | --------------------- |
| timestamp  | integer | unix timestamp is ms  |
| price | float   | trade price           |
| volume| float   | traded quantity       |
| buy   | boolean | true if trade is a buy, false otherwise |

## Examples 

Request the last 20 trades for the binance exchange platform and the symbol BTC/USDT:

```bash
curl https://mnemex.io/api/v1/trades?exchange=binance&symbol=BTC/USDT&nrows=20
```

