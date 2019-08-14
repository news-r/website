# Software

Below are the software developed by news-r, all of which are freely available on [Github](https://github.com/news-r).

## Platforms

Currently only includes one platform which will let you collect and analyse online news and blog coverage generated around topics of your choosing.

- [auritus](https://auritus.io) - Free, open source media monitoring platform (beta)

## Data

The packages below will you collect news articles and information on the latter.

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
- [hoaxy](https://github.com/news-r/hoaxy) - Monitor fake news

## Analysis

The packages below ease the analysis of news articles though they remain rudiementary (for now).

- [gensimr](https://gensimr.news-r.org) - Topic Modeling for Humans
- [word2vec.r](https://word2vec.news-r.org) - Word2vec from Julia to R
- [textanalysis](https://github.com/textanalysis) - TextAnalysis.jl for R
- [webhoserx](https://github.com/news-r/webhoserx) - Feature extraction extension for the `webhoser` package
- [spotlight](https://github.com/news-r/spotlight) - Entity extraction with DBPedia Spotlight
- [decipher](http://decipher.john-coene.com) - Easy natural language processing
- [factcheck](https://github.com/news-r/factcheck) - Fact check queries or publishers

## Go

- [go-webhose](https://github.com/news-r/go-webhose) - webhose.io API

You can install most the above with.

<!-- tabs:start -->

#### ** R **

```r
# install.packages("remotes")
remotes::install_github("news-r/newsr")
```

#### ** Terminal **

```bash
sudo su - -c "R -e \"remotes::install_github('news-r/newsr')\""
```

<!-- tabs:end -->