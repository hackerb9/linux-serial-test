CFLAGS += -Wall

linux-serial-test: linux-serial-test.c bother.c

arm: CC = arm-linux-gnueabi-gcc
arm: linux-serial-test

prefix ?= /usr/local
install: linux-serial-test
	install -D linux-serial-test $(prefix)/bin/

clean:
	rm -f linux-serial-test *.o
