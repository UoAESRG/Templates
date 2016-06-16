# Simple Latex makefile

# Project name, should match .tex and .bib files
NAME=research-proposal

.PHONY: pdf open view edit bib clean

pdf: dir
	latexmk -pdf -jobname=./build/${NAME} ${NAME}.tex

dir:
	mkdir -p build

open: view
view: pdf
	open build/${NAME}.pdf

edit:
	open build/${NAME}.tex

bib:
	open build/${NAME}.bib

clean:
	rm build/*
