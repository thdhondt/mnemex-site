---
title: "Ohlcv"
menutitle: "Ohlcv"
chapter: false
weight: 24
---

## Url

```url
https://mnemex.io/api/v1/ohlcv
```

## Input

| Parameter | Default | Description |
| --------- | ------- | ----------- |
| exchange  | -       | the name of the exchange platform |
| symbol    | -       | the name of the asset pair |
| period    | 60      | resampling period in seconds |
| last      | 100     | the last number of samples to retrieve |
| since     | now     | last timestamp to retrieve the samples from |

## Result

| Field      | Type    | Description |
| ---------- | ------- | ----------- |
| timestamp  | integer | unix timestamp in ms |
| open       | float   | open price |
| high       | float   | high price |
| low        | float   | low price |
| close      | float   | close price |
| vwap       | float   | volume weighted average price |
| count      | integer | number of trades |

## Examples 

```url
https://mnemex.io/api/v1/ohlcv?exchange=kraken&symbol=ETH/BTC&last=20&period=300
```


