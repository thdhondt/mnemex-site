---
title: "statistics"
menutitle: "statistics"
draft: true
weight: 25
---

## Information

URL: https://mnemex.io/api/v1/stats

## Input

| parameters | Default | Description |
| ---------- | ------- | ----------- |
| exchange   | -       | the name of the exchange platform |
| symbol     | -       | the name of the asset pair |
| period     | 60      | resampling period in seconds |
| nrows      | 100     | number of rows |
| last       | now     | last timestamp to retrieve data from |

## Result

| name | type    | description |
| ---- | ------- | ----------- |
| unix | integer | unix timestamp in ms |
| avg  | float   | average trade price |
| std  | float   | standard deviation on the price|
| vwap | float   | volume weighted average price |

## Examples 

Request the last 20 stats for the binance exchange platform and the symbol BTC/USDT:

```
curl https://mnemex.io/api/v1/stats?exchange=binance&symbol=BTC/USDT&period=300&nrows=20
```

