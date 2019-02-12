---
title: "Ohlcv"
menutitle: "Ohlcv"
chapter: false
weight: 24
---

## Information

URL: https://mnemex.io/api/v1/ohlcv

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
| open      | float   | open price |
| high      | float   | high price |
| low       | float   | low price |
| close     | float   | close price |
| vwap      | float   | volume weighted average price |
| count     | integer | number of trades |

## Examples 

Request the last 20 ohlcv for the binance exchange platform and the symbol BTC/USDT:

```bash
curl https://mnemex.io/api/v1/ohlcv?exchange=binance&symbol=BTC/USDT
```


