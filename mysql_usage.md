MYSQL USAGE INSTRUCTIONS
========================

Contents
--------

- [Show databases](#showDatabases)

# Show databases and use a specific database <a name="showDatabases"></a>
```
show databases;
use foo_database;
```

Counting rows
-------------
Count the rows of a specific table
```
select count(*) from footable;
```

Get table column names
----------------------
You can use describe
```
describe footable;
```
On newer versions can use INFORMATION_SCHEMA
```
SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA = 'my_database' AND TABLE_NAME = 'my_table';
```
