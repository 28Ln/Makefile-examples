.PHONY:all
#without_dir= foo.c bar.c main.c
without_dir = $(wildcard *.c)
with_dir:=$(addprefix objs/, $(without_dir))
all:
	@echo $(with_dir)