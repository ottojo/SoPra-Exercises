all: anwendungsfälle.pdf 
	$(info ARTIFACTS:anwendungsfälle.pdf)

anwendungsfälle.pdf: anwendungsfälle.tex tikz-uml.sty
	latexmk -pdf anwendungsfälle.tex	

.PHONY: clean
clean:
	latexmk -C

.PHONY: deploy
deploy: all
	latexmk -c

mkfile_path := $(abspath $(lastword $(MAKEFILE_LIST)))
mkfile_dir := $(dir $(mkfile_path))

tikz-uml.sty:
	wget https://perso.ensta-paris.fr/~kielbasi/tikzuml/var/files/src/tikzuml-v1.0-2016-03-29.tbz
	tar -xf tikzuml-v1.0-2016-03-29.tbz
	cp tikzuml-v1.0-2016-03-29/tikz-uml.sty $(mkfile_dir)/
	rm -r tikzuml-v1.0-2016-03-29
	rm tikzuml-v1.0-2016-03-29.tbz
