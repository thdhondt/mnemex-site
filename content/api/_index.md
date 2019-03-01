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
we gather any trades for several pairs on various exchanges. Why would
you store any trade? Because we simply think that storing candles
can be limiting from a statistical point of view. The data we store must beusefull for data scientists. Therefore being granular is important.

We plan to add orderbooks and spreads in the future. However, those are more memory intensive. We will be glad to provide them to you when Mnemex will have
some more financial support. 

## API endpoints

The following methods are currently supported by the api. 

- timestamp
- exchanges
- symbols
- trades
- ohlcv
- stats

## Call rate

Any Mnemex user can request the database 30 times per minute, i.e. one request every two seconds. This might of course become a limiting factor if you plan to use mnemex do develop a professional application. Note that the API is designed to be a memory, a place were you can find historical data. In case Mnemex reveals itself to be successfull, we will improve this feature for non anonymous users.

## Access

For now, Mnemex is free of charge to any user. 
Accessing the api does not require any password.
Depending on external factors, this last feature might change in the future. 