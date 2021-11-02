# CSV to GZip

Load data from a CSV file to compressed GZip file.  

Plugins:  

- [file-output-plugin]
- [csv-formatter-plugin]
- [gzip-encoder-plugin]
- [bzip2-encoder-plugin]

Generate the complete configuration

```sh
embulk guess seed.yml -o config.yml
```

Run embulk with new configurtation file

```sh
embulk run config.yml
```

<!-- Links -->
[file-output-plugin]: https://github.com/embulk/embulk-docs/blob/master/src/built-in.rst#file-output-plugin
[csv-formatter-plugin]: https://github.com/embulk/embulk-docs/blob/master/src/built-in.rst#csv-formatter-plugin
[gzip-encoder-plugin]: https://github.com/embulk/embulk-docs/blob/master/src/built-in.rst#gzip-encoder-plugin
[bzip2-encoder-plugin]: https://github.com/embulk/embulk-docs/blob/master/src/built-in.rst#bzip2-encoder-plugin
