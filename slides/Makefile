PROJNAME := slides

main:
	Rscript -e 'knitr::Sweave2knitr("slides.Rnw")'
	Rscript -e 'knitr::knit2pdf("slides-knitr.Rnw")'

bib:
	bibtex ${PROJNAME}

clean:
	rm -f *.aux *.blg *.log *.out *.dvi *.lof *.lot
	rm -f *.toc *.nav *.snm *.vrb
	rm -f ${PROJNAME}-knitr.*
	rm -rf figures
