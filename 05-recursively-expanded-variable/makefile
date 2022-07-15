#.PHONY: clean\
all:\
	@echo "MAKE = $(MAKE)"



#.PHONY: all clean\
all clean:\
	@echo "\$$@ = $@"\
	@echo "MAKECMDGOALS = $(MAKECMDGOALS)"


#.PHONY: all\
foo = $(bar)\
bar = $(ugh)\
ugh = Huh?\
all:\
	@echo $(foo)\



#.PHONY: all\
x = foo\
y = $(x) b\
x = later\
xx := foo\
yy := $(xx) b\
xx := later\
all:\
	@echo "x = $(y), xx = $(yy)"


#.PHONY: all\
foo = x\
foo ?= y\
bar ?= y\
all:\
	@echo "foo = $(foo), bar = $(bar)"


#.PHONY: all\
objects = main.o foo.o bar.o utils.o\
objects += another.o\
all:\
	@echo $(objects)



#.PHONY: all\
override foo = x\
all:\
	@echo "foo = $(foo)"

.PHONY: clean
CC = gcc
RM = rm
EXE = simple
OBJS = main.o foo.o
$(EXE): $(OBJS)
	$(CC) -o $@ $^
%.o: %.c
	$(CC) -o $@ -c $^
clean:
	$(RM) $(EXE) $(OBJS)