.PHONY: plain-build ieee-build elsevier-build clean

help:
	@echo "clean-build"
	@echo "plain-build"
	@echo "elsevier-build"
	@echo "ieee-build"

clean:
	rm *.log
	rm *.blg
	rm *.bbl
	rm *.aux

build-all: plain-build ieee-build elsevier-build clean
	plain-build
	ieee-build
	elsevier-build
	clean

plain-build: clean
	pdflatex {{cookiecutter.repo_name}}_Plain
	bibtex {{cookiecutter.repo_name}}_Plain
	pdflatex {{cookiecutter.repo_name}}_Plain
	pdflatex {{cookiecutter.repo_name}}_Plain
	clean

ieee-build: clean
	pdflatex {{cookiecutter.repo_name}}_IEEE
	bibtex {{cookiecutter.repo_name}}_IEEE
	pdflatex {{cookiecutter.repo_name}}_IEEE
	pdflatex {{cookiecutter.repo_name}}_IEEE
	clean

elsevier-build: clean
	pdflatex {{cookiecutter.repo_name}}_Elsevier
	bibtex {{cookiecutter.repo_name}}_Elsevier
	pdflatex {{cookiecutter.repo_name}}_Elsevier
	pdflatex {{cookiecutter.repo_name}}_Elsevier
	clean

word-count:
	wc -wl tex/main.tex


