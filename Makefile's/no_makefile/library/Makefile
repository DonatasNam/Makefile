LIB:= libfile_reader.so
LIB_SRC:= main.c file_reader.c
CFLAGS:= -Wall -fPic -shared
.PHONY: all clean 

all: $(LIB)
$(LIB): $(LIB_SRC)
	$(CC) $(CFLAGS) -o $@ $^
clean:
	$(RM) $(LIB)