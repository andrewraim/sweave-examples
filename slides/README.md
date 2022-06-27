This is an example of Latex slides with embedded R code using Sweave.  The
`knitr` and `tinytex` packages are needed to compile to PDF.  The main slide
source `slides.Rnw` uses `knitr` options in the code chunks; the following pair
commands compiles it into a PDF.

```r
R> knitr::Sweave2knitr("slides.Rnw")
R> knitr::knit2pdf("slides-knitr.Rnw")
```

If the compilation succeeds, the results should be named `slides-knitr.pdf`.

For Rstudio users, note that there is a `Compile PDF` button in the GUI which
can also be used to compile to PDF. This seems to initiate a different series
of commands, which does not make use of `knitr` options in the code chunks as
the above compilation method does.
