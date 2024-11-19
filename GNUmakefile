.POSIX:
.SUFFIXES:
.PHONY: all clean install check

PROJECT   =cgi-scripts
VERSION   =1.0.0
PREFIX    =/usr/local
BUILDDIR ?=.build
UNAME_S  ?=$(shell uname -s)
EXE      ?=$(shell uname -s | awk '/Windows/ || /MSYS/ || /CYG/ { print ".exe" }')

all:
clean:
install:
check:
## -- BLOCK:license --
install: install-license
install-license: README.md COPYING
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp README.md COPYING $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/cgiw $(DESTDIR)$(PREFIX)/bin
	cp bin/md2html_py $(DESTDIR)$(PREFIX)/bin
	cp bin/html_body $(DESTDIR)$(PREFIX)/bin
	cp bin/httpd_pycgi $(DESTDIR)$(PREFIX)/bin
install: install-share
install-share:
	mkdir -p $(DESTDIR)$(PREFIX)/share
	cp -r share/doc $(DESTDIR)$(PREFIX)/share
## -- BLOCK:sh --
