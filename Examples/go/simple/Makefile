TOP        = ../..
SWIG       = $(TOP)/../preinst-swig
SRCS       = simple.c
TARGET     = example
INTERFACE  = example.i

check: build
	$(MAKE) -f $(TOP)/Makefile SRCS='$(SRCS)' TARGET='$(TARGET)' INTERFACE='$(INTERFACE)' go_run

build:
	$(MAKE) -f $(TOP)/Makefile SRCS='$(SRCS)' SWIG='$(SWIG)' \
	TARGET='$(TARGET)' INTERFACE='$(INTERFACE)' go

clean:
	$(MAKE) -f $(TOP)/Makefile INTERFACE='$(INTERFACE)' go_clean
