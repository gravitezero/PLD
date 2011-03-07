SRC = src
TMP = tmp
BIN = bin
TEX_BASE_NAME = main
PDF_BASE_NAME = model

all:
	mkdir -p $(TMP) && cp -r $(SRC)/* $(TMP)/ && cd $(TMP) && pdflatex $(TEX_BASE_NAME).tex && mv $(TEX_BASE_NAME).pdf ../$(BIN)/$(PDF_BASE_NAME).pdf
