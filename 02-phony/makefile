# 如果touch clean,再执行make clean是不会clean的 需要用到.PHONY
#\
all: main.o foo.o\
	gcc -o simple main.o foo.o\
main.o: main.c\
	gcc -o main.o -c main.c\
foo.o: foo.c\
	gcc -o foo.o -c foo.c\
clean:\
	rm simple main.o foo.o

.PHONY: clean
simple: main.o foo.o
	gcc -o simple main.o foo.o
main.o: main.c
	gcc -o main.o -c main.c
foo.o: foo.c
	gcc -o foo.o -c foo.c
clean:
	rm simple main.o foo.o