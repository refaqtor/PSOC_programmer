PROGNAMES=prog

OBJS= prog.o AppData.o DeviceData.o Programmer.o fx2.o utils.o usb.o

INC = -I ../libhex -I ../libini
LIBS = ../libhex/libhex.a ../libini/libini.a -L /usr/local/lib -lusb-1.0

include ../Makefile.inc

prog: $(OBJS)
	$(CXX) $(OBJS) $(LIBS) -o $@

install:: prog
