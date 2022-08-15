# Desenvolvimento Web com Go - Elton Minetto

## GO useful commands

```bash
# list go version
go version

# compile binary file
go build -o bin/main main.go
./bin/main

# compile, execute and delete binary file
go run web/main.go

# format go file
go fmt web/main.go

# test go file
go test web/handlers/beer_test.go

# init go modules manager
go mod init https://github.com/eduardolagolima/curso-desenvolvimento-web-com-go

# add third party package
go get github.com/gorilla/mux
```

## SQLite useful commands

```bash
# create database folder
mkdir data -p

# create and access database file
sqlite3 data/beer.db

# create beer table structure
CREATE TABLE beer (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  name TEXT NOT NULL,
  type INTEGER NOT NULL,
  style INTEGER NOT NULL
);

# list all tables
.tables

# show table schema
.schema beer

# show table structure
PRAGMA table_info(beer);
```
