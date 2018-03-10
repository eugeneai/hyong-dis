.PHONY: all clean

LATEX=lualatex
# LATEX=xelatex

TARGET=synopsis

all: $(TARGET)
	latexmk -pdf -pdflatex="$(LATEX) -shell-escape --synctex=1 %O %S" $<

clean:
	latexmk -C $(TARGET)
	rm -f $(TARGET).bbl
