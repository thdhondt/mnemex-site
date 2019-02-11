---
title: "Postgresql"
date: 2019-02-09T20:31:11+01:00
draft: true
weight: 31
---

## Instal Postgres

Before we install postgres, we should quick perform a quick update of the apt-get repository,

```bash
sudo apt-get update
```

Once apt-get has updated go ahead and download Postgres and its helpful accompanying dependencies,

```bash
sudo apt-get install postgresql postgresql-contrib
```

## Configure Postgres

```bash
sudo su - postgres
```

## Connect to Postgres

```bash
psql -h host -d db_name -U user_name
```

## Usefull commands.

We list here some of the usefull commands,

- List the tables from the public schema:

    ```bash
    >>> \dt
    ```
- List the tables from the schema 'schema':

    ```bash
    >>> \dt "schema".
    ```



