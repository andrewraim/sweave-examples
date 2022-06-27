PROJNAME := article

main:
	Rscript -e 'knitr::Sweave2knitr("${PROJNAME}.Rnw")'
	Rscript -e 'knitr::knit2pdf("${PROJNAME}-knitr.Rnw")'

clean:
	rm -f ${PROJNAME}-knitr.*
	rm -rf figure
