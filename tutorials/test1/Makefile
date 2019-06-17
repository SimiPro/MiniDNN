.PHONY: all
all: test1

# This rule tells make how to build hello from hello.cpp
hello: test1.cpp
	g++ -O2 -I/scratch/gstabile/SISSA_software/MiniDNN/include test1.cpp

# This rule tells make to copy hello to the binaries subdirectory,
# creating it if necessary
.PHONY: install
install:
	mkdir -p binaries
	cp -p test1 binaries

# This rule tells make to delete hello and hello.o
.PHONY: clean 
clean:
	rm -f test1


