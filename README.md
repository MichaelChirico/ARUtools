
<!-- README.md is generated from README.Rmd. Please edit that file -->

# ARUtools <a href="http://arutools.github.io/ARUtools/"><img src="man/figures/logo.png" align="right" height="139" alt="ARUtools website" /></a>

<!-- badges: start -->

[![Codecov test
coverage](https://codecov.io/gh/arutools/ARUtools/branch/main/graph/badge.svg)](https://app.codecov.io/gh/arutools/ARUtools?branch=main)

<!-- badges: end -->

The goal of ARUtools is to facilitate the processing of ARU data and
subsampling of recordings. It remains a development version for now.
What this means for you as a user is that function names and variable
names may change between versions and some functions may become defunct.

## Installation

You can install the current version of ARUtools from the
[R-universe](https://arutools.r-universe.dev/) repository.

``` r
install.packages('ARUtools', repos = 'https://arutools.r-universe.dev/')
```

Alternatively you can install the package from
[GitHub](https://github.com/) with the code below. You will need to have
[Rtools](https://cran.r-project.org/bin/windows/Rtools/rtools43/rtools.html)
installed first:

``` r
# install.packages("pak") # Uncomment if you don't have remotes installed.
pak::pak("arutools/ARUtools")
```

## Learn to use

The easiest way to dig into using the `ARUtools` package is using the
[documentation webpage](https://arutools.github.io/ARUtools/)

There currently are six vignettes that will help you get up and running
with cleaning ARU metadata

- Getting started with ARUtools (`vignette("ARUtools")`)
- Customizing `clean_metadata()` (`vignette("customizing")`)
- Dealing with timezones (`vignette("timezones")`)
- Working with spatial data (`vignette("spatial")`)
- Subsampling recordings (`vignette("SubSample")`)
- Other useful functions (`vignette("Misc")` )

## Provide feedback

If you run into problems or have ideas for extensions, please don’t
hesitate to [submit an
issue](https://github.com/arutools/ARUtools/issues/new/choose).

## Motivation and limitations

This package initially started its life as a series of scripts to
process recordings from multiple large projects around monitoring
migratory bird populations in Ontario’s North.

Moving from scripts to package stemmed from following the wise advice
from Hadley Wickham:

> [A good rule of thumb is to consider writing a function whenever
> you’ve copied and pasted a block of code more than twice (i.e. you now
> have three copies of the same
> code)](https://r4ds.hadley.nz/functions.html#introduction).

With multiple projects, each with their own data issues, it became clear
that this would either require copy/pasting a lot of code and likely
break something or developing a series of functions that could be shared
across projects (i.e. a package).

While that initial version of the code was usable by me and only me, if
you’re using the package, it is because of the fantastic work of [Steffi
LaZerte](https://github.com/steffilazerte) who translated my mess into
the user-friendly functions you see today.

However, due to the variable nature of data management, it is possible
that `ARUtools` may not work well for your project. If you run into
issues, please do submit an issue.

There are also other good packages that may be of use to you:

- [wildRtrax](https://abbiodiversity.github.io/wildRtrax/) (R)
- [seewave](https://search.r-project.org/CRAN/refmans/seewave/html/audiomoth.html)
  (R)
- [warbleR](https://github.com/maRce10/warbleR) (R)
- [emu](https://github.com/QutEcoacoustics/emu) (command line)
- [SoX](https://sourceforge.net/projects/sox/) (command line)
- [Sound-Extraction](https://github.com/prayagnshah/Sound-Extraction)
  (python)
