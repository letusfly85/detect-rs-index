# Show Redshift Index Columns

## Usage

### install 

```
go get github.com/letusfly85/rs-ind-columns
```

### use development.env file

example is below.

```
DB_PARAM="user=USERNAME password=PASSWORD host=HOSTNAME port=PORT_NUMBER dbname=DATABASE_NAME"
```

### run command

`-t` is option to specify table name

```bash
rs-ind-columns -t employee
+------------+-----------------+---------+----------------+
| TABLE NAME |   INDEX NAME    | ATTRNUM |  COLUMN NAME   |
+------------+-----------------+---------+----------------+
| employee   | employee_pkey1  |       2 | employee_id    |
| employee   | employee_pkey1  |       3 | department_id  |
| employee   | employee_pkey1  |       5 | rank_id        |
+------------+-----------------+---------+----------------+
```
