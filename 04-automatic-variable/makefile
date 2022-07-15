.PHONY: clean
CC = gcc
RM = rm
EXE = simple
OBJS = main.o foo.o
$(EXE): $(OBJS)
	$(CC) -o $@ $^
	@echo ">>>> simple:$(CC) -o $@ $^"
main.o: main.c
	$(CC) -o $@ -c $^
	@echo ">>>> main:$(CC) -o $@ -c $^"
foo.o: foo.c
	$(CC) -o $@ -c $^
	@echo ">>>> foo:$(CC) -o $@ -c $^"
clean:
	$(RM) $(EXE) $(OBJS)
	@echo ">>>> clean:$(RM) $(EXE) $(OBJS)"
