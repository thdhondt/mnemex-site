---
title: "Ohlcv"
menutitle: "Ohlcv"
chapter: false
weight: 24
---

## Information

The ohlcv method stands for 'Open High Low Close Vwap'. This one is a classic, every api has it and most of the charts are vizualised as candles. 
Therefore, we had to provide it to you! Although it is very simple to compute it from the raw trades.

The method parameters are the same as for the trades method, except that you can specify the 'period'. The period is simply the amount of time over which you want to agregate a single candle. For further explenations about the othe parameters, please refer to the trades section. 

Note the the period can be any value between 60 seconds and a day, i.e. 86400 seconds. 

## Url

```url
https://mnemex.io/api/v1/ohlcv
```

## Input

| Parameters | Default | Description |
| ---------- | ------- | ----------- |
| exchange   | -       | the name of the exchange platform |
| symbol     | -       | the name of the asset pair |
| period     | 60      | resampling period in seconds |
| last       | 100     | the last number of samples to retrieve |
| since      | now     | last timestamp to retrieve the samples from |

## Result

| Naem      | Type    | Description |
| ----------| ------- | ----------- |
| timestamp | integer | unix timestamp in ms |
| open      | float   | open price |
| high      | float   | high price |
| low       | float   | low price |
| close     | float   | close price |
| vwap      | float   | volume weighted average price |
| count     | integer | number of trades |

## Examples 

Request the last 20 ohlcv for the 'kraken' exchange platform, the 'ETH/BTC' asset pair over a period of time of 5 minutes,

```bash
curl https://mnemex.io/api/v1/ohlcv?exchange=kraken&symbol=ETH/BTC&last=20&period=300
```


