# Database setup

## Setting up Postgres
Follow this:

https://gist.github.com/ibraheem4/ce5ccd3e4d7a65589ce84f2a3b7c23a3

brew services restart postgresql

### Setting up DB and user

Start the postgres command line:
`psql postgres`

Create users and databases:
```
CREATE USER postgres WITH PASSWORD 'postgres';
CREATE DATABASE factsplat_dev
```
(exchange variables depending on what your projects are expecting)
