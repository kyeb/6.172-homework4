#
# Makefile for the qsort example.
#

CC = clang
CFLAGS = -Wall -std=gnu99 -O1 -g -fcilkplus
LDFLAGS = -ldl -lcilkrts

TARGET = qsort
SRC = qsort.c

include ../cilktool/cilkutils.mk

.PHONY: all clean
  
all: $(TARGET)

$(TARGET): $(SRC)
	$(CC) -o $@ $(CFLAGS) $^ $(LDFLAGS)

clean::
	rm -f $(TARGET)
