CC = clang
CFLAGS = -Wall -O3 -g -Werror -gdwarf-3 -std=gnu99 -fcilkplus
LDFLAGS = -ldl -lcilkrts

TARGET = transpose
SRC = transpose.c

include ../cilktool/cilkutils.mk

.PHONY: all clean

all: $(TARGET)

$(TARGET): $(SRC)
	$(CC) -o $@ $(CFLAGS) $^ $(LDFLAGS)

clean::
	rm -f $(TARGET)
