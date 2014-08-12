# Makefile for managing "Lessons In Electric Circuits -- Reference"
# modified  01/7/2006 (DC) -Added mini-TOC  to each chapter of html, .latex
# modified 10/03/2008 (DC) -Added sml2latx.sed, sml2html.sed to Latex and html sections--
#                           -- to for rebuild for changes to these .sed files.


YRES=108

SRC = equation.sml \
      colors.sml \
      citable.sml \
      algebra.sml \
      trig.sml \
      calculus.sml \
      spice.sml \
      trouble.sml \
      symbol.sml \
      periodic.sml \
      about.sml \
      contrib.sml \
      dsl.sml \
      hi.tex \
      bye.tex \
      hi.latex \
      hi_appendix.latex \
      bye.latex \
      hi_1.html \
      hi_2.html \
      hi_3.html \
      hi_4.html \
      hi_5.html \
      hi_6.html \
      hi_7.html \
      hi_8.html \
      hi_9.html \
      hi_10.html \
      hi_A1.html \
      hi_A2.html \
      hi_A3.html \
      bye_1.html \
      bye_2.html \
      bye_3.html \
      bye_4.html \
      bye_5.html \
      bye_6.html \
      bye_7.html \
      bye_8.html \
      bye_9.html \
      bye_10.html \
      bye_A1.html \
      bye_A2.html \
      bye_A3.html \
      index.html \
      Makefile



# Generates HTML output
html : $(SRC) sml2html.sed
	make REF_1.html
	make REF_2.html
	make REF_3.html
	make REF_4.html
	make REF_5.html
	make REF_6.html
	make REF_7.html
	make REF_8.html
	make REF_9.html
	make REF_10.html
	make REF_A1.html
	make REF_A2.html
	make REF_A3.html




# Converts SubML source into TeX source
equation.tex : equation.sml
	sed -f sml2tex.sed equation.sml > equation.tex

colors.tex : colors.sml
	sed -f sml2tex.sed colors.sml > colors.tex

citable.tex : citable.sml
	sed -f sml2tex.sed citable.sml > citable.tex

algebra.tex : algebra.sml
	sed -f sml2tex.sed algebra.sml > algebra.tex

trig.tex : trig.sml
	sed -f sml2tex.sed trig.sml > trig.tex

calculus.tex : calculus.sml
	sed -f sml2tex.sed calculus.sml > calculus.tex

spice.tex : spice.sml
	sed -f sml2tex.sed spice.sml > spice.tex

trouble.tex : trouble.sml
	sed -f sml2tex.sed trouble.sml > trouble.tex

symbol.tex : symbol.sml
	sed -f sml2tex.sed symbol.sml > symbol.tex

periodic.tex : periodic.sml
	sed -f sml2tex.sed periodic.sml > periodic.tex

about.tex : about.sml
	sed -f sml2tex.sed about.sml > about.tex

contrib.tex : contrib.sml
	sed -f sml2tex.sed contrib.sml > contrib.tex

dsl.tex : dsl.sml
	sed -f sml2tex.sed dsl.sml > dsl.tex





# Converts SubML source into LaTeX source
equation.latex : equation.sml sml2latx.sed
	sed -f sml2latx.sed equation.sml > equation.latex

colors.latex : colors.sml sml2latx.sed
	sed -f sml2latx.sed colors.sml > colors.latex

citable.latex : citable.sml sml2latx.sed
	sed -f sml2latx.sed citable.sml > citable.latex

algebra.latex : algebra.sml sml2latx.sed
	sed -f sml2latx.sed algebra.sml > algebra.latex

trig.latex : trig.sml sml2latx.sed
	sed -f sml2latx.sed trig.sml > trig.latex

calculus.latex : calculus.sml sml2latx.sed
	sed -f sml2latx.sed calculus.sml > calculus.latex

spice.latex : spice.sml sml2latx.sed
	sed -f sml2latx.sed spice.sml > spice.latex

trouble.latex : trouble.sml sml2latx.sed
	sed -f sml2latx.sed trouble.sml > trouble.latex

symbol.latex : symbol.sml sml2latx.sed
	sed -f sml2latx.sed symbol.sml > symbol.latex

periodic.latex : periodic.sml sml2latx.sed
	sed -f sml2latx.sed periodic.sml > periodic.latex

about.latex : about.sml sml2latx.sed
	sed -f sml2latx.sed about.sml > about.latex
	#no mini-TOC for this chapter-- remove it
	cp about.latex about.latex~
	sed  s/\\minitoc//g about.latex~ >about.latex

contrib.latex : contrib.sml sml2latx.sed
	sed -f sml2latx.sed contrib.sml > contrib.latex
	#no mini-TOC for this chapter-- remove it
	cp contrib.latex contrib.latex~
	sed  s/\\minitoc//g contrib.latex~ >contrib.latex

dsl.latex : dsl.sml sml2latx.sed
	sed -f sml2latx.sed dsl.sml > dsl.latex
	#no mini-TOC for this chapter-- remove it
	cp dsl.latex dsl.latex~
	sed  s/\\minitoc//g dsl.latex~ >dsl.latex





# Converts SubML source into plain ASCII text
equation.txt : equation.sml
	sed -f sml2txt.sed equation.sml > equation.txt

colors.txt : colors.sml
	sed -f sml2txt.sed colors.sml > colors.txt

citable.txt : citable.sml
	sed -f sml2txt.sed citable.sml > citable.txt

algebra.txt : algebra.sml
	sed -f sml2txt.sed algebra.sml > algebra.txt

trig.txt : trig.sml
	sed -f sml2txt.sed trig.sml > trig.txt

calculus.txt : calculus.sml
	sed -f sml2txt.sed calculus.sml > calculus.txt

spice.txt : spice.sml
	sed -f sml2txt.sed spice.sml > spice.txt

trouble.txt : trouble.sml
	sed -f sml2txt.sed trouble.sml > trouble.txt

symbol.txt : symbol.sml
	sed -f sml2txt.sed symbol.sml > symbol.txt

periodic.txt : periodic.sml
	sed -f sml2txt.sed periodic.sml > periodic.txt

about.txt : about.sml
	sed -f sml2txt.sed about.sml > about.txt

contrib.txt : contrib.sml
	sed -f sml2txt.sed contrib.sml > contrib.txt

dsl.txt : dsl.sml
	sed -f sml2txt.sed dsl.sml > dsl.txt




# Converts SubML source into HTML source
REF_1.html : equation.sml hi_1.html bye_1.html sml2html.sed
	cat hi_1.html > REF_1.html
	sed -f sml2html.sed equation.sml >> REF_1.html
	cat bye_1.html >> REF_1.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_1.html

REF_2.html : colors.sml hi_2.html bye_2.html sml2html.sed
	cat hi_2.html > REF_2.html
	sed -f sml2html.sed colors.sml >> REF_2.html
	cat bye_2.html >> REF_2.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_2.html

REF_3.html : citable.sml hi_3.html bye_3.html sml2html.sed
	cat hi_3.html > REF_3.html
	sed -f sml2html.sed citable.sml >> REF_3.html
	cat bye_3.html >> REF_3.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_3.html

REF_4.html : algebra.sml hi_4.html bye_4.html sml2html.sed
	cat hi_4.html > REF_4.html
	sed -f sml2html.sed algebra.sml >> REF_4.html
	cat bye_4.html >> REF_4.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_4.html

REF_5.html : trig.sml hi_5.html bye_5.html sml2html.sed
	cat hi_5.html > REF_5.html
	sed -f sml2html.sed trig.sml >> REF_5.html
	cat bye_5.html >> REF_5.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_5.html

REF_6.html : calculus.sml hi_6.html bye_6.html sml2html.sed
	cat hi_6.html > REF_6.html
	sed -f sml2html.sed calculus.sml >> REF_6.html
	cat bye_6.html >> REF_6.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_6.html

REF_7.html : spice.sml hi_7.html bye_7.html sml2html.sed
	cat hi_7.html > REF_7.html
	sed -f sml2html.sed spice.sml >> REF_7.html
	cat bye_7.html >> REF_7.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_7.html

REF_8.html : trouble.sml hi_8.html bye_8.html sml2html.sed
	cat hi_8.html > REF_8.html
	sed -f sml2html.sed trouble.sml >> REF_8.html
	cat bye_8.html >> REF_8.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_8.html

REF_9.html : symbol.sml hi_9.html bye_9.html sml2html.sed
	cat hi_9.html > REF_9.html
	sed -f sml2html.sed symbol.sml >> REF_9.html
	cat bye_9.html >> REF_9.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_9.html

REF_10.html : periodic.sml hi_10.html bye_10.html sml2html.sed
	cat hi_10.html > REF_10.html
	sed -f sml2html.sed periodic.sml >> REF_10.html
	cat bye_10.html >> REF_10.html

	./htmltoc2 -inline -noorg  -toclabel " " -tocmap toc.map \
        -minitoc "<\!\-\-\minitoc\-\->" REF_10.html

REF_A1.html : about.sml hi_A1.html bye_A1.html sml2html.sed
	cat hi_A1.html > REF_A1.html
	sed -f sml2html.sed about.sml >> REF_A1.html
	cat bye_A1.html >> REF_A1.html

REF_A2.html : contrib.sml hi_A2.html bye_A2.html sml2html.sed
	cat hi_A2.html > REF_A2.html
	sed -f sml2html.sed contrib.sml >> REF_A2.html
	cat bye_A2.html >> REF_A2.html

REF_A3.html : dsl.sml hi_A3.html bye_A3.html sml2html.sed
	cat hi_A3.html > REF_A3.html
	sed -f sml2html.sed dsl.sml >> REF_A3.html
	cat bye_A3.html >> REF_A3.html



# Generates DVI output using TeX
tex : $(SRC)
	make equation.tex
	make colors.tex
	make citable.tex
	make algebra.tex
	make trig.tex
	make calculus.tex
	make spice.tex
	make trouble.tex
	make symbol.tex
	make periodic.tex
	make about.tex
	make contrib.tex
	make dsl.tex
	cat hi.tex \
           equation.tex \
           colors.tex \
           citable.tex \
           algebra.tex \
           trig.tex \
           calculus.tex \
           spice.tex \
           trouble.tex \
           symbol.tex \
           periodic.tex \
           about.tex \
           contrib.tex \
           dsl.tex \
           bye.tex > REF.tex
	tex REF.tex
	touch tex





# Generates DVI output using LaTeX
latex : $(SRC) sml2latx.sed
	make equation.latex
	make colors.latex
	make citable.latex
	make algebra.latex
	make trig.latex
	make calculus.latex
	make spice.latex
	make trouble.latex
	make symbol.latex
	make periodic.latex
	make about.latex
	make contrib.latex
	make dsl.latex
	cat hi.latex \
           equation.latex \
           colors.latex \
           citable.latex \
           algebra.latex \
           trig.latex \
           calculus.latex \
           spice.latex \
           trouble.latex \
           symbol.latex \
           periodic.latex \
           hi_appendix.latex \
           about.latex \
           contrib.latex \
           dsl.latex \
           bye.latex > REF.latex
	latex REF.latex
	makeindex REF.idx
	latex REF.latex
	latex REF.latex
	touch latex






# Generates plain ASCII output
txt : $(SRC)
	make equation.txt
	make colors.txt
	make citable.txt
	make algebra.txt
	make trig.txt
	make calculus.txt
	make spice.txt
	make trouble.txt
	make symbol.txt
	make periodic.txt
	make about.txt
	make contrib.txt
	make dsl.txt
	cat equation.txt \
           colors.txt \
           citable.txt \
           algebra.txt \
           trig.txt \
           calculus.txt \
           spice.txt \
           trouble.txt \
           symbol.txt \
           periodic.txt \
           about.txt \
           contrib.txt \
           dsl.txt > REF.txt
	touch txt




# Generates compressed PostScript and PDF output
REF.ps : $(SRC)
	make latex
	dvips -z -Ppdf -o REF.ps REF.dvi
	ps2pdf REF.ps REF.pdf
	gzip -f REF.ps




# Converts schematic and equation .eps graphics into .png format
png: $(SRC)
	mogrify -density 120 -format png 0*.eps
	mogrify -density 120 -format png 1*.eps
	touch png


# Converts photograph .jpg graphics into .eps format
# Don't have png2eps? Then use eps2: target instead of eps: target It
# only needs mogrify. But images files are larger, Images not as nice.
# This (eps2: or eps:) is only required for TeX/LaTeX.

eps2: $(SRC)
	mogrify -density 175 -format eps 4*.jpg
	mogrify -density 175 -format eps 5*.jpg
	touch eps





# Convert *.jpg to .eps -smaller .eps files than above, alternative to above


eps: $(SRC)
	YRES=108  #Y resolution to shrink height, 72 normal
	for file in 2*.png; do \
	../bin/png2eps $$file $(YRES) >`echo $$file | sed -ne 's/png/eps/p;'`; \
	done

	for file in 5*.jpg; do \
	cp $$file $$file'~' ; \
	done

	for file in 4*.jpg; do \
	cp $$file $$file'~' ; \
	done

	../bin/jpeg2eps 4*.jpg
	../bin/jpeg2eps 5*.jpg


	for file in 4*.eps; do \
	cp $$file $$file'~' ; \
	done

	for file in 5*.eps; do \
	cp $$file $$file'~' ; \
	done

	for file in 4*.eps; do \
	../bin/./scale.sh 50% $$file'~' $$file ; \
	done

	for file in 5*.eps; do \
	../bin/./scale.sh 50% $$file'~' $$file ; \
	done

#	modify for each directory
	rm 41*.jpg~
	rm 51*.jpg~
	rm 41*.eps~
	rm 51*.eps~
	touch eps






# Generates a .tar.gz archive containing source files
REFsrc.tar.gz: $(SRC)
	tar cvf REFsrc.tar \
            $(SRC) \
            *.eps \
            *.jpg \
            *.png \
            *.lps \
            *.sed \
            toc.map \
            htmltoc2 \
            Makefile
	gzip -f REFsrc.tar




# Generates a .tar.gz archive containing only ESSENTIAL source files
REFtiny.tar.gz: $(SRC)
	tar cvf REFtiny.tar \
            $(SRC) \
            0*.eps \
            1*.eps \
            4*.jpg \
            5*.jpg \
            previous.jpg \
            contents.jpg \
            next.jpg \
            ps.* \
            pdf.* \
            src1.* \
            src2.* \
            *.lps \
            *.sed \
            toc.map \
            htmltoc2 \
            Makefile
	gzip -f REFtiny.tar


# Cleans out old, unwanted files
clean:
	-rm *.bak
	-rm *.spn
	-rm junk*
	-rm core

