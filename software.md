# Software

Below are the packages included in 

## Platforms

- [auritus](auritus.io)

## APIs

- [newsapi](https://github.com/news-r/newsapi) - newsapi.org
- [guardian](https://github.com/news-r/guardian) - The Guardian API
- [papers](https://github.com/news-r/papers) - Information on newspapers
- [loc](https://github.com/news-r/loc) - Library of Congress API
- [webhoser](https://github.com/news-r/webhoser) - webhose.io API
- [webhoserx](https://github.com/news-r/webhoserx) - Feature extraction extension for `webhoser`
- [currents](https://github.com/news-r/currents) - Currents API
- [nytimes](https://github.com/news-r/nytimes) - New York Times API
- [spotlight](https://github.com/news-r/spotlight) - Entity extraction with DBPedia Spotlight
- [stocknews](https://github.com/news-r/stocknews) - Stocknews API (financial news)
- [ft](https://github.com/news-r/ft) - Financial Times API
- [accunews](https://github.com/news-r/accunews) - AccuNews API (local news)

## Analysis

```r
# install.packages("remotes")
remotes::install_github("news-r/newsr")

# load libraries
library(newsr)

news <- search_news("query")
```