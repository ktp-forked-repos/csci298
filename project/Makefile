CFLAGS=-g -D_GNU_SOURCE -std=c99 -lncurses

crr: crrses.o handlers.o reservations.o rooms.o signals.o crr.o -lncurses

tar: crr.tar.bz2

crr.tar.bz2: *.c *.h
	tar -cjf crr.tar.bz2 *.{h,c} Makefile rooms.dat

.PHONY: clean
clean:
	$(RM) crr *.o *.tar.bz2
