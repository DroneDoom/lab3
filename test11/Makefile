CC=g++
CFLAGS=-c -g -Wall -DNDEBUG
LDFLAGS= -lUnitTest++
SOURCES= main.cpp modAlphaCipher.cpp
HEADERS =	modAlphaCipher.h
OBJECTS=$(SOURCES:.cpp=.o)
EXECUTABLE=testing

all: $(SOURCES) $(EXECUTABLE)
	
$(EXECUTABLE): $(OBJECTS) 
	$(CC) $(OBJECTS) -o $@ $(LDFLAGS)

.cpp.o:
	$(CC) $(CFLAGS) $< -o $@
clean:
	rm $(OBJECTS) $(EXECUTABLE)
