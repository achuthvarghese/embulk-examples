# CSV to PostgreSQL

Load data from a CSV file to a PostgreSQL database table.  

Required plugins:

- [embulk-output-postgresql]

Install plugin

```sh
embulk gem install embulk-output-postgresql
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
[embulk-output-postgresql]: https://github.com/embulk/embulk-output-jdbc/tree/master/embulk-output-postgresql
