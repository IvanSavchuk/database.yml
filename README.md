<h1> Configuring a MySQL or MariaDB Database </h1>

If you choose to use `MySQL` or `MariaDB` instead of the shipped `SQLite3` database, 
your config/database.yml will look a little different. 
Here's the development section:

```
development:
  adapter: mysql2
  encoding: utf8
  database: blog_development
  pool: 5
  username: root
  password:
  socket: /tmp/mysql.sock
```
If your development database has a root user with an empty password, this configuration should work for you. 
Otherwise, change the username and password in the development section as appropriate.
