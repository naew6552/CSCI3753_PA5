# File : Makefile
# By: Nate Ewan
# CSCI 3753 PA 5
# Description:
#   Makefile for PA5

CC           = gcc

CFLAGSFUSE   = `pkg-config fuse --cflags`
LLIBSFUSE    = `pkg-config fuse --libs`
LLIBSOPENSSL = -lcrypto

CFLAGS	     = -c -g -Wall -Wextra
LFLAGS	     = -g -Wall -Wextra

ENC_FS = encfs

encfs : encfs.o
    $(CC) $(LFLAGS) $^ -o $@ $(LLIBSFUSE) 

encfs.o : encfs.c
    $(CC) $(CFLAGS) $(CLFAGSFUSE) $<

clean:
