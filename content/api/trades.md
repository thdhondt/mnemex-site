---
title: "Trades"
menutitle: "Trades"
chapter: false
weight: 23
---

## Information

This method makes all the trades available to you, from now until we started collecting data. You can choose the exchange and the asset pair, or symbol. 
Simple requesting the url with an exchange and a symbol returns the last 100 trades. If you want to broaden the window, the parameter last can be increased up to one hundred. If you want to request the 'last' n trades since a specific timestamp, the 'since' parameter can be specified. Its default value is now. 

## Url

```url
https://mnemex.io/api/v1/trades
```

## Input

| Parameters | Default | Description |
| ---------- | ------- | ----------- |
| exchange   | -       | the name of the exchange platform |
| symbol     | -       | the name of the asset pair |
| last       | 100    | the last number of samples to retrieve |
| since      | now     | the timestamp to retrieve the samples from |

## Result

| Name  | Type    | Description |
| ----- | ------- | ----------- |
| timestamp  | integer | unix timestamp is ms  |
| price  | float | trade price |
| volume | float | traded quantity |
| buy    | boolean | true if the trade is a buy, false otherwise |

## Examples 

Request the last 50 ohlcv for the 'kraken' exchange platform, the 'ETH/BTC' asset pair over a period of time of 5 minutes,

```bash
curl https://mnemex.io/api/v1/trades?exchange=kraken&symbol=ETH/BTC&last=50
```

