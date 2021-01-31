main.pdf: DustJacket/DustJacket.pdf main.tex arati.tex lotus.png prakkathana.tex uttarardha.tex sampadakiya_two.tex sampadakiya.tex ss.tex uttarardha.tex \
          Cambay-Bold.ttf Cambay-BoldItalic.ttf Cambay-Italic.ttf Cambay-Regular.ttf \
          CharisSILB.ttf CharisSILBI.ttf CharisSILI.ttf CharisSILR.ttf arialunicodems.ttf
	latexmk -pdfxe main.tex
	# latexmk -c main.tex  # Doesn't remove the .xdv file

clean:
	rm -f -v main.{aux,fdb_latexmk,fls,log,toc,xdv}

diff:
	diff-pdf --skip-identical --mark-differences --view main-Cambay.pdf main.pdf

# Not part of any target:
#   COPYING
#   Makefile (this file)
#   README
#   "Śrībhaktamāla (Mūlārthabodhinī Ṭīkā Sahita) 2nd Edition.pdf" (=canonical version of main.pdf)
