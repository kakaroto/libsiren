ACLOCAL_AMFLAGS = -Im4 -Wall -Wextra

lib_LTLIBRARIES = libsiren.la

libsiren_la_SOURCES = \
	common.c dct4.c decoder.c encoder.c huffman.c \
	huffman.h rmlt.h common.h dct4.h decoder.h \
	encoder.h huffman_consts.h rmlt.c siren7.h

libsiren_la_LIBADD =  $(LIBM)
libsiren_la_LDFLAGS = $(LIBSIREN_LT_LDFLAGS)


pkginclude_HEADERS = siren7.h encoder.h decoder.h

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = libsiren.pc

