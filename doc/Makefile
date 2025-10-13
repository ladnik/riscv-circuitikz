# TEXS := $(wildcard *.tex)
TEXS := manual.tex

.PHONY: all clean distclean

# compile a specific .tex file to PDF and clean auxiliary files
%.pdf: %.tex figures/*.tikz ../tikzlibraryriscvproc.code.tex
	TEXINPUTS=../: pdflatex -interaction=nonstopmode -shell-escape $<
	TEXINPUTS=../: pdflatex -interaction=nonstopmode -shell-escape $<

# compile all .tex files
all: $(TEXS:.tex=.pdf)

# clean auxiliary files
clean:
	rm -f *.aux *.log *.out *.toc *.nav *.snm *.vrb *.synctex.gz *.fls *.fdb_latexmk *.bak* *.tmp

# clean all output files
distclean: clean
	rm -f $(TEXS:.tex=.pdf)
