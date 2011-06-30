GRAPHVIZ = dot

prefix = ../OEBPS

all: svg

svg: $(prefix)/compile.svg

MV = mv
$(prefix)/compile.svg: compile.svg
	$(MV) $^ $@

%.svg: %.dot
	$(GRAPHVIZ) -Tsvg -o $@ $^
