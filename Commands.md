### PostgreSQL
- `psql --username=freecodecamp --dbname=second_database;`
- `\l` view all the databases
- `\d` display the feautures and details of a table
- `SELECT * FROM ({table_name});` shows what is inside the table
- `CREATE DATABASE {databasename};`
- `DROP DATABASE databasename;`
- `CREATE TABLE table_name (
    column1 datatype,
    column2 datatype,
    column3 datatype,
   ....
);`
- `DROP TABLE table_name`
- `ALTER TABLE table_name ADD COLUMN column_name TYPE;`
- `ALTER TABLE second_table RENAME COLUMN name TO username;` 
- `INSERT INTO table_name(column_1, column_2) VALUES(value1, value2);` entering data 
- `SELECT columns FROM table_name;` Viewing data
- `DELETE FROM table_name WHERE condition;`
- `ALTER DATABASE database_name RENAME TO new_database_name;`
- `\c database_name` change to another database
- `ALTER TABLE table_name ADD PRIMARY KEY(column_name);`
- `ALTER TABLE table_name ADD COLUMN column_name DATATYPE REFERENCES referenced_table_name(referenced_column_name);`
- `ALTER TABLE {table_name} ADD UNIQE({column_name});`
- `ALTER TABLE table_name ALTER COLUMN column_name SET NOT NULL;`
- `ALTER TABLE table_name ADD COLUMN column_name DATATYPE CONSTRAINT REFERENCES referenced_table_name(referenced_column_name);`
- `ALTER TABLE table_name ADD FOREIGN KEY(column_name) REFERENCES referenced_table(referenced_column);`
- `SELECT * FROM table_1 FULL JOIN table_2 ON table_1.primary_key_column = table_2.foreign_key_column;`

```
SELECT columns FROM junction_table
FULL JOIN table_1 ON junction_table.foreign_key_column = table_1.primary_key_column
FULL JOIN table_2 ON junction_table.foreign_key_column = table_2.primary_key_column;
```
