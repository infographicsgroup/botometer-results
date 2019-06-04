# DATA

This is a selection of the scraped data (as at May 29 2019).

`index` as Excel and TSV gives an overview of the published data. It contains a list of 21 Twitter lists, that should be 100% humans, and 2 lists of Twitter accounts, that should be 100% bots.
Each line also includes a summary of the botometer results.

For convenience we also added a link to the original data source e.g. the Twitter list.

## files

You can find the results in the folders `humans` and `bots`.

For every scanned list we have two files:
1. `?.ndjson.xz` is a new line delimited file of JSONs. Every JSON contains the raw data from the Twitter API, and the results of the botometer. The whole file is compressed with XZ, a LZMA based, very high efficient, open source compressor. You can find a decompressor for XZ for every platform. You might wanna check if your current decompressor already understands XZ.
2. `?.tsv` is a new line delimited, tab separated table of the results. It can be imported to e.g. Excel.