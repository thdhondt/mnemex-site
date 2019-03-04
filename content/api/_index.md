---
title: "Api"
menuTitle: "Api"
chapter: false
weight: 20
---

Mnemex is built to be scalable. Only few exchanges and
and symbols are currently supported by the api. We plan
of course the enrich the database in the future. Memory cost is the limit
but we can virtually support any exchange and pairs that are supported by CCXT. 

## Data

What do we store in the database? Well it is very simple for now, 
we gather trades for several pairs on various exchanges. We plan to add orderbooks and spreads in the future. However, those are more memory intensive. 

## API endpoints

The following methods are currently supported by the api. 

- timestamp
- exchanges
- symbols
- trades
- ohlcv
- stats

## Call rate

Any Mnemex user can request the database 30 times per minute, i.e. one request every two seconds. This might of course become a limiting factor if you plan to use mnemex do develop a professional application. Note that the API is designed to be a place where you can find historical data for amateur projects. 

## Access

For now, Mnemex is free of charge to any user. 
Accessing the api does not require any password.
Depending on external factors, this last feature might change in the future. 
