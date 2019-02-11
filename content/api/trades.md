---
title: "trades"
menutitle: "trades"
draft: true
weight: 23
---

## Information

URL: https://mnemex.io/api/v1/trades

WARNING: This routine is under maintenance!

## Input

| parameters | Default | Description |
| ---------- | ------- | ----------- |
| exchange   | -       | the name of the exchange platform |
| symbol     | -       | the name of the asset pair |
| nrows      | 100     | number of rows |
| last       | now     | last timestamp to retrieve data from |

## Result

| name  | type    | description           |
| ----- | ------- | --------------------- |
| unix  | integer | unix timestamp is ms  |
| price | float   | trade price           |
| volume| float   | traded quantity       |
| buy   | boolean | true if trade is a buy, false otherwise |

## Examples 

Request the last 20 trades for the binance exchange platform and the symbol BTC/USDT:

```
curl https://mnemex.io/api/v1/trades?exchange=binance&symbol=BTC/USDT&nrows=20
```

