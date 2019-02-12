---
title: "Statistics"
menutitle: "Statistics"
chapter: false
weight: 24
---

## Information

URL: https://mnemex.io/api/v1/stats

## Input

| parameters | default | description |
| ---------- | ------- | ----------- |
| exchange   | -       | the name of the exchange platform |
| symbol     | -       | the name of the asset pair |
| period     | 60      | resampling period in seconds |
| limit      | 1000    | number of samples to retrieve |
| since      | now     | last timestamp to retrieve the data from |

## Result

| name      | type    | description |
| ----------| ------- | ----------- |
| timestamp | integer | unix timestamp in ms |
| avg       | float   | average trade price |
| std       | float   | standard deviation on the price |
| vwap      | float   | volume weighted average price |
| qty       | float   | sum of the traded volume |

## Examples 

Request the last 20 stats for the binance exchange platform and the symbol BTC/USDT:

```bash
curl https://mnemex.io/api/v1/stats?exchange=binance&symbol=BTC/USDT
```

