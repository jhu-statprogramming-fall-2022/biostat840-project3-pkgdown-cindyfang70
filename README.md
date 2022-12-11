# gridExtra

[pkgdown website](https://jhu-statprogramming-fall-2022.github.io/biostat840-project3-pkgdown-cindyfang70/), built by Xin Zhi (Cindy) Fang.

[Original gridExtra repo](https://github.com/baptiste/gridExtra), built by Baptiste Auguie.

Five customized things:

- changed the bootswatch theme to `cerulean`
- changed the background, foreground, and primary colours of the site
- changed the base font of the site
- changed the spacing between the nav bar and the main text
- changed the theme of the code blocks

Exported functions:

- `arrangeGrob`: arrange multiple plots on a page
- `bind`: perform `rbind` or `cbind` on `gtable` objects
- `combine`: combine `gtable` objects based on their row or column names.
- `ngongGrob`: create regular polygon `grob` objects that can be rotated and stretched.
- `tableGrob`: graphically display text `grob` objects.

Example usage:
```
library(gridExtra)
library(grid)
library(ggplot2)
library(lattice)
p <- qplot(1,1)
p2 <- xyplot(1~1)
r <- rectGrob(gp=gpar(fill="grey90"))
t <- textGrob("text")
grid.arrange(t, p, p2, r, ncol=2)
```


[![Build Status](https://travis-ci.org/baptiste/gridextra.svg?branch=master)](https://travis-ci.org/baptiste/gridextra)
[![](http://www.r-pkg.org/badges/version/gridExtra)](https://CRAN.R-project.org/package=gridExtra )
[![](http://cranlogs.r-pkg.org/badges/grand-total/gridExtra)](http://cran.rstudio.com/web/packages/gridExtra/index.html)

[![R build status](https://github.com/baptiste/gridextra/workflows/R-CMD-check/badge.svg)](https://github.com/baptiste/gridextra/actions)

Provides a number of user-level functions to work with "grid" graphics, notably to arrange multiple grid-based plots on a page, and draw tables. Earlier versions of the package contained more experimental graphical objects (grobs), that have now been removed.

See the [gridExtra wiki](https://github.com/baptiste/gridextra/wiki) for additional information, answers to Frequently Asked Questions, and the latest vignettes.

[![DOI](https://zenodo.org/badge/5734/baptiste/gridextra.png)](http://dx.doi.org/10.5281/zenodo.11422)


