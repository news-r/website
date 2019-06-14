# news-r

`news-r` is an initiative creating tools to improve the collection and analysis of the traditional media. Its ultimate aim being to simultaneously increase press scrutiny and freedom of information.

Thus far the initiative has focused on easing access to data useful to its endeavour, pimarily in the R programming language (some in Go). Though several such data sources have been approached already (including [The Guardian](https://github.com/news-r/guardian) and [The New York Times](https://github.com/news-r/nytimes)) many more need to be made accessible to researchers.

Once all major sources are integrated with the R language, `news-r` aims at unifying the them into one single API for convenience.  

```r
# install.packages("remotes")
remotes::install_github("news-r/newsr")

# load libraries
library(newsr)
```

The above R command installs and loads the packages listen below.

```r
#> ── Attaching newsr ───────────────────────────────────────── newsr 0.0.1 ──
#> ✔ newsapi   0.0.1          ✔ webhoserx 0.0.1     
#> ✔ guardian  0.0.1.9000     ✔ currents  0.0.1     
#> ✔ papers    0.0.0.9000     ✔ nytimes   0.0.0.9000
#> ✔ loc       0.0.0.9000     ✔ spotlight 0.0.0.9000
#> ✔ webhoser  0.0.1          ✔ stocknews 0.0.1     
#> ✔ accunews  0.0.1          ✔ ft        0.0.1
```