PROJNAME := slides

main:
	Rscript -e 'knitr::Sweave2knitr("slides.Rnw")'
	Rscript -e 'knitr::knit2pdf("slides-knitr.Rnw")'

clean:
	rm -f ${PROJNAME}-knitr.*
	rm -rf figure
