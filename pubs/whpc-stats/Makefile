ifndef SYSCONF_HOME
$(error SYSCONF_HOME environment variable is not set)
endif

export

all: stats.pdf

stats.pdf: $(wildcard *.Rmd) Makefile ../sysconf.bib ../load_data.R
	$(R) -e 'library(bookdown); bookdown::render_book("stats.Rmd", "bookdown::pdf_book")'
	mv _book/_main.pdf $@

clean:
	$(R) -e 'bookdown::clean_book(clean = T)'
	rm -rf stats.pdf stats.tex _main.* libs _book _bookdown_files *.html *.log *.aux *.bbl *.blg *.dvi *.out *.xcp
