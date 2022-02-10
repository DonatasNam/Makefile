exec:= program
BIN:= main.o maths.o usage.o
BIN_SRC:= main.c maths.c usage.c
CFLAGS:= -Wall
CPPFLAGS= -I.
LDFLAGS= -L.

.PHONY: all clean
all: $(exec)

$(exec):$(BIN)
	$(CC) $(CFLAGS) -o $@ $^ 

$(BIN):$(BIN_SRC)
	$(CC) $(LDFLAGS) $(CPPFLAGS) $(CFLAGS) -c $^ -libfile_reader

clean:
	$(RM) $(BIN) $(exec)