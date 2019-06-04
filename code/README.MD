# CODE

The scraper to get the botometer scores is part of a bigger framework. Unfortunately I can’t publish the whole framework because it uses hundreds of donated Twitter API tokens. For security reasons we can’t publish them.
Without them you can’t use the system. :(

But what we can do is:
1. link to the original code base of the framework: https://github.com/MichaelKreil/twitter-analysis
2. publish the code parts that were used to scrape the botometer scores.

## Scraper

### 1_scan.js

This is the scraper.

The function `scanUsers` is the central function that scans every account of a list, fetches the botometer score and saves the raw data as `.ndjson.xz` and a summary of the results as `.tsv`.

### botometer.js

… is references by `1_scan.js` in line 11 as library.

It scrapes the user information (line 16), the user timeline (line 20) and the mentions (line 24), then sends a request to the botometer API (line 30) and returns everything.


