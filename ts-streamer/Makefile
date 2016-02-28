#
# Makefile to build TeamSpeak 3 SDK Client Sample on Mac OS X
#

CFLAGS = -Wall -g -O0

all: ts-streamer

ts-streamer: main.o
	gcc -o ts-streamer main.o -Linclude/ -lts3client_mac -L/usr/local/lib -lmp3lame.0

main.o: main.c
	gcc -c -Iinclude main.c $(CFLAGS)

clean:
	rm -rf *.o ts-streamer
