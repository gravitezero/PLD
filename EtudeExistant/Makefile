SRC = src
TMP = tmp
BIN = bin
TEX_BASE_NAME = main
PDF_BASE_NAME = Etude\ de\ l\'Existant

all:
	mkdir -p $(TMP) ; \
	for i in AnalyseExistant NormesBench Cible ; do \
	mkdir -p $(TMP)/$$i ; \
	cp -r $$i/$(SRC)/* $(TMP)/$$i/ ; \
	done ; \
	cp -r $(SRC)/* $(TMP)/ ; \
	cd $(TMP) ; \
	pdflatex $(TEX_BASE_NAME).tex ; \
	mv $(TEX_BASE_NAME).pdf ../$(BIN)/$(PDF_BASE_NAME).pdf
