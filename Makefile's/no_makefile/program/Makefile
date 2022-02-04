BIN:= main.o maths.o usage.o
BIN_SRC:= main.c maths.c usage.c
HEAD:= maths.h usage.h
PREF:= ./no_makefile
LD_LIBRARY_PATH=`pwd`./usage.h `pwd`./maths.h
.PHONY: all clean
all: $(BIN)

$(BIN):$(BIN_SRC)
	$(CC) -I. -L. -Wall -o $@ $^ -l_prog

clean:
	$(RM) $(BIN)