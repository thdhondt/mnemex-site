---
title: "Statistics"
menutitle: "Statistics"
chapter: false
weight: 25
---

## Url

```url
https://mnemex.io/api/v1/stats
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
| avg        | float   | average trade price |
| std        | float   | standard deviation on the price |
| vwap       | float   | volume weighted average price |
| qty        | float   | sum of the traded volume |

## Examples 

```url
curl https://mnemex.io/api/v1/stats?exchange=kraken&symbol=ETH/BTC&last=20&period=300
```

