# Generated automatically from Makefile.in by configure.
# === GNUmakefile ============================================================
# Copyright (c) 1993 Chris Provenzano, proven@athena.mit.edu
#
#	Description: This file is for creating the test programs for libpthread.a
#
#	1.00 93/08/03 proven
#		-Initial cut for pthreads.
#

CC = ../pgcc -notinstalled
srctop = /home/my/tmp/BUILD/mit-pthreads
srcdir = /home/my/tmp/BUILD/mit-pthreads/lib
VPATH = /home/my/tmp/BUILD/mit-pthreads/lib
CDEBUGFLAGS = -O3 -DDBUG_OFF   -Werror

CFLAGS = $(CDEBUGFLAGS) $(INCLUDES) $(ADDL_CFLAGS) -DSRCDIR=\"$(srcdir)\"

#
DIRS = libpthreadutil

################################################################################
#
all:
	(for i in $(DIRS); do cd $$i; $(MAKE) all; cd ..; done)

clean: 
	(for i in $(DIRS); do cd $$i; $(MAKE) clean; cd ..; done)
	rm -f *.o $(TESTS) $(BENCHMARKS) a.out core maketmp makeout

depend:
	(for i in $(DIRS); do cd $$i; $(MAKE) depend; cd ..; done)
	sed '/\#\#\# Dependencies/q' < Makefile > maketmp
	(for i in $(CSRC);do $(CPP) -M $$i;done) >> maketmp
	cp maketmp Makefile

install:
	(for i in $(DIRS); do cd $$i; $(MAKE) install; cd ..; done)

realclean: clean
	(for i in $(DIRS); do cd $$i; $(MAKE) realclean; cd ..; done)
	rm -f Makefile

Makefile: Makefile.in
	(cd .. ; sh config.status)

################################################################################
### Do not remove the following line. It is for depend #########################
### Dependencies:
