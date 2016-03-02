obj-m     := hello.o

KERNELDIR ?= /lib/modules/$(shell uname -r)/build
PWD       := $(shell pwd)

all:
	$(MAKE) -C $(KERNELDIR) M=$(PWD)

clean:
	rm -rf *.o *.ko .*.cmd *.mod.c *.order *.symvers .tmp_versions
