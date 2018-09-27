CXX = g++
CXXFLAGS	= -std=c++11 -Wall
CXXTESTFLAGS = --coverage # can be used to generate files that help calculate unit test coverage
CXXGDB = -ggdb

all: animal

clean:
	rm animal # Rectangle.o (because you can't recompile this one!)

animal: Animal.o main.cpp
	$(CXX) $(CXXFLAGS) main.cpp Animal.o -o animal

Animal.o: Animal.cpp
	$(CXX) $(CXXFLAGS) -c Animal.cpp
