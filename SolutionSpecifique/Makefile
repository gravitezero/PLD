SRC = src
TMP = tmp
BIN = bin
IMG = img
TEX_BASE_NAME = main
PDF_BASE_NAME = Expression\ des\ Besoins

all:
	mkdir -p $(TMP) ; \
	for i in ArchitectureTechnique ArchitectureLogicielle ArchitectureApplicative NouvelleOrganisation; do \
	mkdir -p $(TMP)/$$i ; \
	cp $$i/$(SRC)/* $(TMP)/$$i/ ; \
	cp -r $$i/$(SRC)/$(IMG)/ $(TMP)/ ; \
	done ; \
	cp -r $(SRC)/* $(TMP)/ ; \
	cd $(TMP) ; \
	pdflatex $(TEX_BASE_NAME).tex ; \
	mv $(TEX_BASE_NAME).pdf ../$(BIN)/$(PDF_BASE_NAME).pdf
