# Database setup

## Setup in Docker

This may not be necessary. Maybe you're running things in Docker instead:
"Docker Desktop for Apple silicon also supports multi-platform images, which allows you to build and run images for both x86 and ARM architectures without having to set up a complex cross-compilation development environment."

### Neo4j

How to run Neo4j in Docker:
https://neo4j.com/developer/docker-run-neo4j/

I first set it up with an older version simulated with amd. Then a DB was created. I had to drop that database in order to start from scratch, by going to the console at localhost:7474, using username 'neo4j' and password 'test'.
Drop database:
`DROP DATABASE graph.db`
Create new database:
`CREATE DATABASE graph.db`

See this for more DB commands: https://neo4j.com/docs/cypher-manual/current/databases/ 

According to some people the Neo4j 4.4 version supports the new M1 processors.
https://githubmemory.com/repo/neo4j/neo4j/issues/12692?page=2

If you have problems, this one might help: https://rajfal.github.io/2018/Create-a-clean-Neo4j-database-inside-Docker-container/

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

