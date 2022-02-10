CC:=gcc
CFLAGS:= -fpic -shared -Wall
LIB:=libcalculator.so
CFILES:= math_functions.c
.PHONY: all install uninstall clean
all: $(LIB)

$(LIB):$(CFILES)
	$(CC) $(CFLAGS) -o $@ $^

install: $(LIB)
	install -m 644 math_functions.h /usr/include
	install -m 644 libcalculator.so /usr/lib
uninstall:
	$(RM) /usr/include/math_functions.h
	$(RM) /usr/lib/libcalculator.so
clean: 
	$(RM) $(LIB) 
