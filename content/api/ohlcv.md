---
title: "ohlcv"
menutitle: "ohlcv"
draft: true
weight: 24
---

## Information

URL: https://mnemex.io/api/v1/ohlcv

{{% notice warning %}}
This routine is under maintenance!
{{% /notice %}}

## Input

| parameters | default | description |
| ---------- | ------- | ----------- |
| exchange   | -       | the name of the exchange platform |
| symbol     | -       | the name of the asset pair |
| period     | 60      | resampling period in seconds |
| nrows      | 100     | number of rows |
| last       | now     | last timestamp to retrieve data from |

## Result

| name  | type    | description |
| ----- | ------- | ----------- |
| unix  | integer | unix timestamp in ms |
| open  | float   | open price |
| high  | float   | high price |
| low   | float   | low price |
| close | float   | close price |
| count | integer | number of trades |

## Examples 

Request the last 20 ohlcv for the binance exchange platform and the symbol BTC/USDT:

```
curl https://mnemex.io/api/v1/ohlcv?exchange=binance&symbol=BTC/USDT&period=300&nrows=20
```


