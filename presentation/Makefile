TEX_IMAGE=xelatex
TEX_IMAGE_TAG=full

all:
	docker run --rm -v $(PWD):$(PWD) -w $(PWD) $(TEX_IMAGE):$(TEX_IMAGE_TAG) xelatex presentation.tex

bib:
	docker run --rm -v $(PWD):$(PWD) -w $(PWD) $(TEX_IMAGE):$(TEX_IMAGE_TAG) bibtex presentation

clean:
	rm -f presentation.{aux,bbl,blg,log,out,toc,lot,lof}

full: clean all bib
	docker run --rm -v $(PWD):$(PWD) -w $(PWD) $(TEX_IMAGE):$(TEX_IMAGE_TAG) xelatex presentation.tex
	docker run --rm -v $(PWD):$(PWD) -w $(PWD) $(TEX_IMAGE):$(TEX_IMAGE_TAG) xelatex presentation.tex

read:
	epdfview presentation.pdf
