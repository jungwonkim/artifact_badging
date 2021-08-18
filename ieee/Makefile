SAMPLE=sample_ieee

all: draft

draft: $(SAMPLE).tex
	latexmk -pdf $(SAMPLE)

clean:
	latexmk -C; rm -f $(SAMPLE).bbl $(SAMPLE).pdf

