# Variables
CC = gcc
CFLAGS = -Wall -Wextra -std=c11
OBJDIR = obj
BINDIR = bin
TARGET = $(BINDIR)/main
SRCS = main.c
OBJS = $(OBJDIR)/main.o

# Rules
all: $(TARGET)

$(TARGET): $(OBJS)
	@mkdir -p $(BINDIR)
	$(CC) $(CFLAGS) -o $@ $^

$(OBJDIR)/%.o: %.c
	@mkdir -p $(OBJDIR)
	$(CC) $(CFLAGS) -c -o $@ $<

clean:
	rm -rf $(OBJDIR) $(BINDIR)

.PHONY: all clean