## Process this file with automake to produce Makefile.in

## Created by Anjuta

AM_CPPFLAGS = \
	-DPACKAGE_LOCALE_DIR=\""$(localedir)"\" \
	-DPACKAGE_SRC_DIR=\""$(srcdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(pkgdatadir)"\"

AM_CFLAGS =\
	 -Wall\
	 -g

lib_LTLIBRARIES = libdecnumber.la


libdecnumber_la_SOURCES = \
	decNumber.c \
	decContext.c \
	decDouble.c \
	decimal32.c \
	decimal64.c \
	decimal128.c \
	decPacked.c \
	decQuad.c \
	decSingle.c

libdecnumber_la_LDFLAGS = 

libdecnumber_la_LIBADD = 


if PLATFORM_WIN32
libdecnumber_la_LDFLAGS += -no-undefined
endif

if NATIVE_WIN32
libdecnumber_la_LDFLAGS += -export-dynamic
endif

include_HEADERS = \
	decCommon.c \
	decBasic.c \
	decContext.h \
	decDouble.h \
	decDPD.h \
	decimal32.h \
	decimal64.h \
	decimal128.h \
	decNumber.h \
	decNumberLocal.h \
	decPacked.h \
	decQuad.h \
	decSingle.h

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = libdecnumber-3.68.pc

EXTRA_DIST = \
	libdecnumber-3.68.pc.in
