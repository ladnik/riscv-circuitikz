TEXS := $(wildcard *.tex)
LIB := $(realpath ../lib/tikzlibraryriscvproc.code.tex)

LATEXMKFLAGS+=-pdf -halt-on-error -interaction=nonstopmode -shell-escape

.PHONY: all clean distclean

# compile a specific .tex file to PDF and clean auxiliary files
%.pdf: %.tex $(LIB)
	TEXINPUTS=../lib//: latexmk $(LATEXMKFLAGS) $<

# compile all .tex files
all: $(TEXS:.tex=.pdf)

# clean auxiliary files
clean:
	rm -f *.aux *.log *.out *.toc *.nav *.snm *.vrb *.synctex.gz *.fls *.fdb_latexmk *.bak* *.tmp

# clean all output files
distclean: clean
	rm -f $(TEXS:.tex=.pdf)
