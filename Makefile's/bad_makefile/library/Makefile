CC:=gcc
CFLAGS:= -I. -fpic -shared -Wall
LIB:=calculator.so
CFILES:= math_functions.c
PREFIX:= /`pwd`
.PHONY: all install uninstall clean
all: $(LIB)

$(LIB):$(CFILES)
	$(CC) $(CFLAGS) -o $@ $^

install: $(LIB)
	install -d $(DESTDIR) $(PREFIX)/include
	install -m 644 math_functions.h $(DESTDIR)/$(PREFIX)/include

uninstall:
	$(RM) $(DESTDIR)/$(PREFIX)/include/math_functions.h

clean: 
	rm -f $(LIB) math_functions.o
