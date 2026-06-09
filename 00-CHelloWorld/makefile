CC := gcc
CFLAGS := -std=c11 -Wall -Wextra
SRC := hello.c
TARGET := hello

.PHONY: all build run output clean

all: build

build: $(SRC)
	$(CC) $(CFLAGS) -o $(TARGET) $(SRC)

run: build
	./$(TARGET)

output: build
	./$(TARGET) > output.txt

clean:
	rm -f $(TARGET) $(TARGET).exe output.txt
