#.PHONY: all\
sharp = square\
desk = square\
table = circle\
 \
ifeq ($(sharp), $(desk))\
	result1 = "desk == sharp"\
endif\
ifneq "$(table)" 'square'\
	result2 = "table != square"\
endif\
all:\
	@echo $(result1)\
	@echo $(result2)
	
.PHONY: all
foo = defined
ifdef foo
	result1 = "foo is defined"
endif
ifndef bar
	result2 = "bar is not defined"
endif
all:
	@echo $(result1)
	@echo $(result2)
