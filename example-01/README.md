# CSV to StdOut

Load data from a CSV file in a GZIP file and output it to stdout.  

![example-01-00.png]

Generate the complete configuration

```sh
embulk guess seed.yml -o config.yml
```

Run embulk with new configurtation file

```sh
embulk run config.yml
```

Just by changing the `path_prefix` in [seed.yml] to `'./data/sample_'` from `'./data/compressed_'` we can see the change in the configuration file generated. A decoder of type gzip is removed from the configuration by finding out that the file is of type CSV.  

When CSV file is detected:  
![example-01-01.png]

When GZip file is detected:  
![example-01-02.png]

<!-- Links -->
[seed.yml]: ./seed.yml

<!-- Images -->
[example-01-00.png]: ../screenshots/example-01-00.png
[example-01-01.png]: ../screenshots/example-01-01.png
[example-01-02.png]: ../screenshots/example-01-02.png
