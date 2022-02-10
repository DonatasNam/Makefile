CPPFLAGS:= -I.
CFLAGS:= -Wall -Ipwd
CFILES:= math_functions.c main.c
BIN:= calculator

.PHONY: all clean

all: $(BIN)

$(BIN): $(CFILES)
	$(CC) $(CPPFLAGS) $(CFLAGS) -o $@ $^

clean:
	$(RM) $(BIN) 
