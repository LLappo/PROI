all: main.out

.PHONY: release debug clean

CC = $(CXX)
CXXFLAGS = -Wall -Wextra -std=c++11

release: CXXFLAGS += -O2
release: main.out

debug: CXXFLAGS += -g -O0
debug: main.out

main: main.o class.o

main.o: main.cpp class.h

class.o: class.cpp class.h

clean:
	rm -rf *.o