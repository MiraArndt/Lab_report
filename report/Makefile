all: build/thesis.pdf

.PRECIOUS: build/thesis.pdf

TeXOptions = -pvc \
			 -lualatex \
			 -output-directory=build \
	  	     -interaction=errorstopmode \


build/thesis.pdf: FORCE | build
	latexmk $(TeXOptions) thesis.tex
	
FORCE:

build:
	mkdir -p build/

clean:
	rm -rf build