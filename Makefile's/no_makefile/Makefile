.PHONY: library program clean all

all: library program

library:
	$(MAKE) -C ./library

program:
	$(MAKE) -C ./program

clean:
	$(MAKE) -C ./library clean
	$(MAKE) -C ./program clean