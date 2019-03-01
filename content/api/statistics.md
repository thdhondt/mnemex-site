---
title: "Statistics"
menutitle: "Statistics"
chapter: false
weight: 25
---

## Information

The stats method stands simply for 'Statistcs'. Here, we provide you the averaged trade price, the standard deviation for that one, the volume weighted average price and the sum of the quantities over a certain amount of time defined by the 'period' parameter. For more information about the method parameters, please refer to the trades section.

## Url

```url
https://mnemex.io/api/v1/stats
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

| Name      | Type    | Description |
| ----------| ------- | ----------- |
| timestamp | integer | unix timestamp in ms |
| avg       | float   | average trade price |
| std       | float   | standard deviation on the price |
| vwap      | float   | volume weighted average price |
| qty       | float   | sum of the traded volume |

## Examples 

Request the last 20 stats for the 'kraken' exchange platform, the 'ETH/BTC' asset pair over a period of time of 5 minutes,

```bash
curl https://mnemex.io/api/v1/stats?exchange=kraken&symbol=ETH/BTC&last=20&period=300
```

