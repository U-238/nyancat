OBJECTS = nyancat.o music.o

CC	?=
CFLAGS	 ?= -g -Wall -Wextra -std=c99 -pedantic -Wwrite-strings -Wno-incompatible-pointer-types-discards-qualifiers -Wno-unused-parameter -Wno-discarded-qualifiers -Wno-unknown-warning-option
CPPFLAGS ?=
LDFLAGS  ?= -lsox -lpthread

all: nyancat

nyancat: $(OBJECTS)
	$(CC) $(CPPFLAGS) $(CFLAGS) $(LDFLAGS) $(OBJECTS) -o $@

clean:
	-rm -f $(OBJECTS) nyancat

check: all
	# Unit tests go here. None currently.
	@echo "*** ALL TESTS PASSED ***"

.PHONY: all clean check
