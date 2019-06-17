# Contributing

<mark>If you are visiting this page, thank you for even contemplating a contribution.</mark>

Pretty much anyone is of course welcome to contribute to the initiative. Please report any bug you encounter or suggest any feature by opening Github issues. Also feel free to contribute on any [Github](https://github.com/news-r) software by creating pull requests.

Then of course there are other contriutions which I omitted to mention, e.g. if you can design, a logo would great. The only thing that is not accepted currently is money.

## Coding Standards

If you intend to contribute to anything code-related please try to abide by the style guide as much as you can.

First keep the package name all lowercase. 

Use the package [assertthat](https://github.com/hadley/assertthat) for assertions (namely of inputs) over the base R `if` and `stop` combination. If you are integrating an API with R use a setup function called `packageName_key` which sets the `key` as an environment variable named `PACKAGENAME_API_KEY` (with `Sys.setenv()`). Below is how it is implemented in the [newsapi](https://github.com/news-r/newsapi) package.

```r
ft_key <- function(key){
  assert_that(!missing(key), msg = "Missing key")
  Sys.setenv(NEWSAPI_API_KEY = key)
}
```

This allows users to setup their key in their `.Renviron` file, which is easily done with `usethis::edit_r_environ()`. This is why such packages also print messages when attaching the package to let the user know whether the key was found and loaded.

```r
.onAttach <- function(...) {
  key <- Sys.getenv("NEWSAPI_API_KEY")

  msg <- "No API key found, see `newsapi_key`"
  if(nchar(key) > 1) msg <- "API key loaded!"

  packageStartupMessage(msg)
}
```

Then generally this key is accessed with `Sys.getenv()` internally.

To make various API calls use either [httr](https://github.com/r-lib/httr) or, if the API allows large number of calls, [async](https://github.com/r-lib/async), currently only the package [guardian](https://github.com/news-r/guardian) makes use of the latter.

Try, where possible to return a `tibble` instead of a `list`.

## Style

Below is the main color palette used.

<span style="background:#247BA0;" class="palette">#247BA0</span>
<span style="background:#70C1B3;" class="palette">#70C1B3</span>
<span style="background:#B2DBBF;" class="palette">#B2DBBF</span>
<span style="background:#F3FFBD;" class="palette">#F3FFBD</span>
<span style="background:#FF1654;" class="palette">#FF1654</span>

The background color of this page is #f9f7f1 while the font is <span style="background:#2f2f2f;" class="palette">#2f2f2f</span> in [Playfair Display](https://fonts.google.com/specimen/Playfair+Display).