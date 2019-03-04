---
title: "Trades"
menutitle: "Trades"
chapter: false
weight: 23
---

## Url

```url
https://mnemex.io/api/v1/trades
```

## Input

| Parameter | Default | Description |
| --------- | ------- | ----------- |
| exchange  | -       | the name of the exchange platform |
| symbol    | -       | the name of the asset pair |
| last      | 100    | the last number of samples to retrieve |
| since     | now     | the timestamp to retrieve the samples from |

## Result

| Field      | Type    | Description |
| ---------- | ------- | ----------- |
| timestamp  | integer | unix timestamp is ms  |
| price      | float   | trade price |
| volume     | float   | traded quantity |
| buy        | boolean | true if the trade is a buy, false otherwise |

## Examples 

```url
https://mnemex.io/api/v1/trades?exchange=kraken&symbol=ETH/BTC&last=20
```

