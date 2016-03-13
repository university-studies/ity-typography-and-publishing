NAME=proj4

all:
	vlna -v -f $(NAME).bib $(NAME).bib
	vlna -v -f $(NAME).tex $(NAME).tex

	latex $(NAME).tex
	
	bibtex $(NAME).aux
	
	latex $(NAME).tex
	latex $(NAME).tex
	dvips -t a4 $(NAME).dvi
	ps2pdf $(NAME).ps


clean:
	rm -f $(NAME).aux $(NAME).bbl $(NAME).blg $(NAME).dvi $(NAME).log $(NAME).ps $(NAME).pdf

pack: 
	zip xloffa00-fit.zip Makefile proj4.tex czechiso.bst citacie.bib