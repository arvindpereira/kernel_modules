obj-m		+= mmap_kernel_simple.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules
	#gcc -o user_test -c user_test.c

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
	rm user_test
