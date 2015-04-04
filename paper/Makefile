NAME =paper
TEX_SRC =$(NAME).tex

all: $(NAME).pdf

PDFLATEX =pdflatex --shell-escape $(TEX_SRC)

$(NAME).pdf: *.tex
	$(PDFLATEX)
	bibtex $(NAME).aux
	$(PDFLATEX)
	$(PDFLATEX)
	rm -rf *.log *.aux *.toc *.ps *.mps *.dvi *.pyg.* *.bbl *.blg *.out

clean:
	rm -rf *.log *.aux *.toc *.dvi *.ps *.pdf *.mps *.pyg.* *.bbl *.blg *.out

