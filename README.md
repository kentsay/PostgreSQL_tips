# PostgreSQL_tips
Tips of using PostgreSQL
---

| MySQL command        | PostgreSQL equivalent	           | Description|
| ---------------------|:---------------------------------:| ----------:|
| SHOW DATABASES;      | \list            | Show databases |
| USE some_database;   | \c some_database | Use/Connect to a database named 'some_database' |
| SHOW TABLES;         | \dt              | Show tables/relations within one database |
| DESCRIBE some_table; | \d+ some_table   | Show table details (columns, types) |
| SHOW INDEX FROM some_table; | \di       | Show indices of some_table (in case of MySQL) and all indices of database (PostgreSQL) |
| CREATE USER harry IDENTIFIED BY 'foo'; | CREATE ROLE username WITH createdb LOGIN PASSWORD 'password';      |    Create user that can create databases |
| … | ALTER ROLE username WITH PASSWORD 'password';      |    Change password of an existing user |
| GRANT ALL PRIVILEGES ON database.* TO username@localhost; | GRANT ALL PRIVILEGES ON DATABASE database TO username;      |    Grants access to a database. |
| ? | ALTER USER username CREATEDB;      |    Grants access to create databases. |

