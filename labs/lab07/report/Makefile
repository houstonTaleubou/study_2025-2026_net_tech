FILES = $(patsubst %.md, %.docx, $(wildcard *.md))
FILES += $(patsubst %.md, %.pdf, $(wildcard *.md))

FILTERS =
OPTIONS = --number-sections --resource-path=.:image
PDF_ENGINE = --pdf-engine=lualatex --pdf-engine-opt=--shell-escape
PDF_OPTIONS =
FORMAT_OPTIONS =

# Opções de bibliografia (removidas temporariamente)
# BIB_OPTIONS = --citeproc
# PDF_BIB_OPTIONS = --citeproc
BIB_OPTIONS =
PDF_BIB_OPTIONS =

%.docx: %.md
	-pandoc "$<" $(FILTERS) $(OPTIONS) $(BIB_OPTIONS) -o "$@"

%.pdf: %.md
	-pandoc "$<" $(FILTERS) $(PDF_ENGINE) $(PDF_OPTIONS) $(PDF_BIB_OPTIONS) $(FORMAT_OPTIONS) $(OPTIONS) -o "$@"

all: $(FILES)

clean:
	-rm -f $(FILES) *~

cleanall: clean

.PHONY: all clean cleanall
