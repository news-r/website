# Software

Below are the packages included in 

## Platforms

- [auritus](https://auritus.io) - Free, open source media monitoring platform (beta)

## Data

- [newsapi](https://github.com/news-r/newsapi) - newsapi.org
- [guardian](https://github.com/news-r/guardian) - The Guardian API
- [papers](https://github.com/news-r/papers) - Information on world wide newspapers
- [loc](https://github.com/news-r/loc) - Library of Congress API
- [webhoser](https://github.com/news-r/webhoser) - webhose.io API
- [currents](https://github.com/news-r/currents) - Currents API
- [nytimes](https://github.com/news-r/nytimes) - New York Times API
- [stocknews](https://github.com/news-r/stocknews) - Stocknews API (financial news)
- [ft](https://github.com/news-r/ft) - Financial Times API
- [accunews](https://github.com/news-r/accunews) - AccuNews API (local news)
- [greatfire](https://github.com/news-r/greatfire) - Keywords and URLs Censored on the Chinese Internet

## Analysis

- [webhoserx](https://github.com/news-r/webhoserx) - Feature extraction extension for the `webhoser` package
- [spotlight](https://github.com/news-r/spotlight) - Entity extraction with DBPedia Spotlight
- [decipher](http://decipher.john-coene.com) - Easy natural language processing

## Go

- [go-webhose](https://github.com/news-r/go-webhose) - webhose.io API

You can install the above with.

```r
# install.packages("remotes")
remotes::install_github("news-r/newsr")

# load libraries
library(newsr)

news <- search_news("query")
```