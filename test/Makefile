CC        := gcc
LIBS      := -llogdb -lpthread 
LDFLAGS   := -L ../ -L.
INCLUDE   := -I ../include
CFLAGS    := -g -O0  -Wall
SRCS := $(wildcard *.c)
TARGET  := $(patsubst %.c, %, $(SRCS))
OBJDIR = .

.c:
	$(CC) $(CFLAGS)   -o $@ $<   $(INCLUDE) $(LDFLAGS) $(LIBS)
all: $(TARGET) 
clean:
	rm -rf *.o
	rm -rf dump stress check_pwrite_o_append