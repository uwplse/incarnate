JSRC = $(wildcard *.java)

all: GCodeAnalyzer.class

GCodeAnalyzer.class: $(JSRC)
	javac GCodeAnalyzer.java

test: GCodeAnalyzer.class
	./test.sh

test-slic3r: GCodeAnalyzer.class
	./test-slic3r.sh

clean:
	rm -f *.class

.PHONY: test test-slic3r clean
