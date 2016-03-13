NAME=proj5

all:
	vlna -v -f $(NAME).tex $(NAME).tex
	
	latex $(NAME).tex
	latex $(NAME).tex
	dvips -t a4 $(NAME).dvi
	ps2pdf $(NAME).ps


clean:
	rm -f $(NAME).aux  $(NAME).blg $(NAME).dvi $(NAME).log $(NAME).ps $(NAME).pdf $(NAME).out

pack: 
	zip xloffa00-fit.zip Makefile proj5.tex PPRfyma2.sty lezec.eps horolezec.eps
