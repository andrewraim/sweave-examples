Sweave provides a way to embed R code in Latex documents. R users may be more
familiar with Rmarkdown which provides similar functionality in Markdown
documents. This repo contains simple Sweave examples in an article format and
Beamer slides.

The documents support Sweave through `knitr`
(<https://yihui.org/knitr/demo/sweave/>). Compiling them requires the `knitr`
and `tinytex` packages. The following pair of R commands can be used to
compile the article from its `Rnw` source to a PDF.

```r
R> knitr::Sweave2knitr("article.Rnw")
R> knitr::knit2pdf("article-knitr.Rnw")
```

If the compilation succeeds, the results should be named `articld-knitr.pdf`.
A similar pair of commands can be used to compile the slides.

A `Makefile` is included with each document which can be used to build the
respective PDF from a Unix command line.

For Rstudio users, note that there is a `Compile PDF` button in the GUI which
can also be used to compile to PDF. This seems to initiate a different series
of commands, which does not make use of `knitr` options in the code chunks as
the above compilation method does.



