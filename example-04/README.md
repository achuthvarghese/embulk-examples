# PostgreSQL to MySQL

Load data from a PostgreSQL database table to a MySQL database table.  

Prerequisites:  
Import user_profiles.sql into PostgreSQL database using Adminer UI after running docker-compose.

Required plugins:

- [embulk-input-postgresql]
- [embulk-output-mysql]

Install plugin

```sh
embulk gem install embulk-input-postgresql embulk-output-mysql 
```

Generate the complete configuration

```sh
embulk guess seed.yml -o config.yml
```

Run embulk with new configurtation file

```sh
embulk run config.yml
```

<!-- Links -->
[embulk-input-postgresql]: https://github.com/embulk/embulk-input-jdbc/tree/master/embulk-input-postgresql
[embulk-output-mysql]: https://github.com/embulk/embulk-output-jdbc/tree/master/embulk-output-mysql
