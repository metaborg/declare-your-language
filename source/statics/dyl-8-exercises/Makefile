## Optionally add extra latex source folders (must end with colon!)
export TEXINPUTS = texmf/:

LATEXMK   = latexmk -r latexmkrc

.SUFFIXES: .pdf

.PRECIOUS: build/%.pdf

%.pdf: build/%.pdf
	cp "$<" "$@"

build/%.pdf: %.tex FORCE
	$(LATEXMK) "$<"

.PHONY: all bib clean

all: document.pdf

clean:
	$(LATEXMK) -C

FORCE:
