## TechBBS bot

Tracks new sell listings on TechBBS

---

> This assumes you already have a MariaDB instance set up and running

Get the source code and setup python environment using pipenv:
```
$ git clone https://joinemm/techbbs-bott
$ cd techbbs-bot
$ pipenv install
```

Fill out the `config.toml.example` with your own values and rename it to `config.toml`.

Build the database schema:
```
[]> CREATE DATABASE dbname;
$ mysql dbname < sql/schema.sql
```

If everything went well you should be able to run the bot with

```
$ pipenv run python main.py
```
