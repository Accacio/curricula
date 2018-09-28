all: pt en fr clean
	cp *.pdf ../

clean:
	./clean_latex.sh

pt:
	pdflatex -jobname cv-Rafael_Accacio_NOGUEIRA-pt "\AtBeginDocument{\portuguese}\input{curriculum-multilingual.tex}" 
	zathura cv-Rafael_Accacio_NOGUEIRA-pt.pdf &

en: 
	pdflatex -jobname cv-Rafael_Accacio_NOGUEIRA-en "\AtBeginDocument{\english}\input{curriculum-multilingual.tex}"
	zathura cv-Rafael_Accacio_NOGUEIRA-en.pdf &

fr: 
	pdflatex -jobname cv-Rafael_Accacio_NOGUEIRA-fr "\AtBeginDocument{\french}\input{curriculum-multilingual.tex}"
	zathura cv-Rafael_Accacio_NOGUEIRA-fr.pdf &
