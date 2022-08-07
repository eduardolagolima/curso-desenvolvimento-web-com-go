# curso-desenvolvimento-web-com-go

## GO useful commands

```bash
# compile binary file
go build -o bin/main main.go
./bin/main

# compile, execute and delete binary file
go run main.go

# format go file
go fmt main.go
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
