all: main.pdf

DustJacket.pdf: DustJacket.tex Bhaktamala2.png logo2.png \
                ChanakyaSanskrit-Bold.ttf ChanakyaSanskrit-BoldItalic.ttf ChanakyaSanskrit-Italic.ttf ChanakyaSanskrit-Regular.ttf \
                CharisSILB.ttf CharisSILBI.ttf CharisSILI.ttf CharisSILR.ttf arialunicodems.ttf \
                Rupee_Foradian.ttf
	latexmk -pdfxe DustJacket.tex
	rm -f -v DustJacket.{aux,fdb_latexmk,fls,log,out,toc,xdv}

main.pdf: DustJacket.pdf main.tex arati.tex lotus.png prakkathana.tex uttarardha.tex sampadakiya_two.tex sampadakiya.tex ss.tex uttarardha.tex \
          ChanakyaSanskrit-Bold.ttf ChanakyaSanskrit-BoldItalic.ttf ChanakyaSanskrit-Italic.ttf ChanakyaSanskrit-Regular.ttf \
          CharisSILB.ttf CharisSILBI.ttf CharisSILI.ttf CharisSILR.ttf arialunicodems.ttf
	latexmk -pdfxe main.tex
	# latexmk -c main.tex  # Doesn't remove the .xdv file
	rm -f -v main.{aux,fdb_latexmk,fls,log,toc,xdv}

# Not part of any target:
#   COPYING
#   Makefile (this file)
#   README
#   "Śrībhaktamāla (Mūlārthabodhinī Ṭīkā Sahita) 2nd Edition.pdf" (=canonical version of main.pdf)
