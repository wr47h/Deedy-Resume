TEX_FILE		 = RodolfoFerro.xtx
PDF_FILE		 = RodolfoFerro.pdf
CACHE_DIR   := $(shell pwd)/.latex-cache
COMPILE_TEX := latexmk -xelatex $(TEX_FILE) -output-directory=$(CACHE_DIR)

run:
	$(COMPILE_TEX)
	@cp $(CACHE_DIR)/$(notdir $(PDF_FILE)) $(PDF_FILE)
	@rm -rf "$(CACHE_DIR)"
