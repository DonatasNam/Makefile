LIB:= libfile_reader.so
LIB_SRC:= main.c file_reader.c
LIB_INC:= file_reader.h
.PHONY: all clean 

all: $(LIB)
$(LIB): $(LIB_SRC)
	$(CC) -I. -Wall -o $@ $^
clean:
	$(RM) $(LIB)