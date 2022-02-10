CPPFLAGS:= -I.
CFLAGS:= -Wall -Ipwd
CFILES:= math_functions.c main.c
BIN:= calculator

.PHONY: all clean

all: $(BIN)

$(BIN): $(CFILES)
	$(CC) $(Flags) -o $@ $^

clean:
	$(RM) $(BIN) 
