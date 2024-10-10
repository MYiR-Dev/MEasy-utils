CC ?= $(CROSS_COMPILE)gcc
#TARGET = $(notdir $(CURDIR))_test
#SRC =  $(shell ls *.c)
#OBJS = $(patsubst %.c ,%.o ,$(SRC))
#.PHONY: all
#all: $(TARGET)
#$(TARGET) : $(OBJS)
#	$(CC) -o $@ $^
#%.o : %.c
#	$(CC) -c $< -o $@
#clean:
#	$(RM) *.o $(TARGET)
SRCS = rs485_read.c rs485_write.c
TARGET = rs485_read rs485_write
all: $(TARGET)

rs485_read: rs485_read.c
	$(CC) -o $@ $^

rs485_write: rs485_write.c
	$(CC) -o $@ $^

clean:
	$(RM) *.o $(TARGET)
.PHONY: all clean
