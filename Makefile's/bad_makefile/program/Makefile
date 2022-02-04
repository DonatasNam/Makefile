compiler:=gcc
Flags:= -I. -L. -Wall -Ipwd
OBJS:=main.o math_functions.o
CFILES:= math_functions.c main.c
BIN:= calculator
all: $(BIN)

$(BIN): $(CFILES)
	$(compiler) $(Flags) -o $@ $^

clean:
	rm -f $(BIN) $(OBJS)
