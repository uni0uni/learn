obj-m := diamorphine.o
CC = gcc -Wall 
KDIR := /lib/modules/$(shell uname -r)/build
# or if you installed headers in /usr/src:
# KDIR := /usr/src/linux-4.19
PWD := $(shell pwd)

all:
	$(MAKE) -C $(KDIR) M=$(PWD) modules

clean:
	$(MAKE) -C $(KDIR) M=$(PWD) clean
