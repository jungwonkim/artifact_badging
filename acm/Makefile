SAMPLE=sample_acm

all: draft

draft: $(SAMPLE).tex
	latexmk -pdf $(SAMPLE)

clean:
	latexmk -C; rm -f $(SAMPLE).bbl $(SAMPLE).pdf

