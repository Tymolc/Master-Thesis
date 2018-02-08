THESIS=masterthesis

all:
	pdflatex ${THESIS}.tex
	ack "(Reference|Citation).*undefined" ${THESIS}.log; true

refs:
	pdflatex ${THESIS}.tex && bibtex ${THESIS} && pdflatex ${THESIS}.tex
	fixme

fixme:
	ack "(Reference|Citation).*undefined" ${THESIS}.log
