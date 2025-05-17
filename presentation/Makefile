clean:
	rm -f pdf/presentation.pdf
	rm -f presentation.*
	rm -f tex/*.aux

all: tex/*.tex bib/bibliography.bib
	pdflatex base/presentation.tex
	bibtex presentation
	pdflatex base/presentation
	pdflatex base/presentation
	mv presentation.pdf pdf/presentation.pdf
	rm -f presentation.*
	rm -f tex/*.aux
	rm -f base/*.log