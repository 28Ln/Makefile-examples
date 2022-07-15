#.PHONY:all\
MKDIR=mkdir\
DIRS=objs exes\
all:$(DIRS)




#.PHONY:all\
MKDIR=mkdir\
RM=rm\
DIRS=objs exes\
all:$(DIRS)\
$(DIRS):\
	$(MKDIR) $@

.PHONY:all
MKDIR=mkdir
DIRS=objs exes
RM=rm
RMFLAGS=-rf
all:$(DIRS)
$(DIRS):
	$(MKDIR) $@
clean:
	$(RM) $(RMFLAGS) $(DIRS)
 