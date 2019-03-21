TMP_SUFFS   = aux bbl blg log

all: main clean
	main
	clean


main:
	pdflatex -interaction=nonstopmode main
	bibtex main
	pdflatex -interaction=nonstopmode main


clean:
	rm -rf $(foreach suff, ${TMP_SUFFS}, main.${suff})
