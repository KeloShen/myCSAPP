CC = gcc
ICS = ..
CFLAGS = -Wall -Og -m64

PROGS = hello hello.i hello.s hello.o hello_unlink.s hello_link.s

all: $(PROGS)

# Precompile
hello.i: hello.c
	$(CC) $(CFLAGS) -E hello.c -o hello.i

# Compile to assembly
hello.s: hello.i
	$(CC) $(CFLAGS) -S hello.i -o hello.s

# Compile to object file
hello.o: hello.s
	$(CC) $(CFLAGS) -c hello.s -o hello.o

# Link to create executable
hello: hello.o
	$(CC) $(CFLAGS) -o hello hello.o
	

# To see what linker does, we can compare the disassembly of the object file before linking and the executable after linking.
# Disassemble object file of hello.o which is not linked yet
hello_unlink.s: hello.o
	objdump -d hello.o > hello_unlink.s
# Disassemble the linked executable hello
hello_link.s: hello
	objdump -d hello > hello_link.s


clean:
	rm -f $(PROGS) hello *.o *~ hello.i hello.s