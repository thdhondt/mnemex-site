---
title: "Timescaledb"
date: 2019-02-09T20:31:20+01:00
draft: true
weight: 32
---

## Install Timescale

You fill find extensive installation about the installation of TimescaleDB on Ubuntu [here](https://docs.timescale.com/v1.2/getting-started/installation/docker/installation-ap-ubuntu)

## Create a Timescale Extension

Start by connecting to your database a super user:

```sql
psql -U postgres -d database
```

then create the extesion:
```sql
CREATE EXTENSION IF NOT EXISTS timescaledb CASCADE;
```

Your are all set!

## Api reference

The api reference for the timescale project is well explained [here](https://docs.timescale.com/v1.2/api#create_hypertable).


