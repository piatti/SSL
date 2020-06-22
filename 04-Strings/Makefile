CC=gcc
CFLAGS= -g -Wall

default: all
all: app

string: String.h String.c StringTest.c
	$(CC) string String.c StringTest.c
  
clean: -rm -f app
