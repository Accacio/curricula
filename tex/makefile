all: pt en fr clean
	cp *.pdf ../

clean:
	./clean_latex.sh

pt:
	pdflatex -jobname cv-Rafael_Accacio_NOGUEIRA-pt "\AtBeginDocument{\selectlanguage{portuguese}}\input{curriculum-multilingual.tex}"

vpt: pt
	zathura cv-Rafael_Accacio_NOGUEIRA-pt.pdf &

en: 
	pdflatex -jobname cv-Rafael_Accacio_NOGUEIRA-en "\AtBeginDocument{\selectlanguage{english}}\input{curriculum-multilingual.tex}"

ven: en
	zathura cv-Rafael_Accacio_NOGUEIRA-en.pdf &

fr: 
	pdflatex -jobname cv-Rafael_Accacio_NOGUEIRA-fr "\AtBeginDocument{\selectlanguage{french}}\input{curriculum-multilingual.tex}"

vfr: fr
	zathura cv-Rafael_Accacio_NOGUEIRA-fr.pdf &
