AUTOMAKE_OPTIONS = subdir-objects

noinst_LIBRARIES         	= libfko_util.a

libfko_util_source_files 	= \
    ../lib/strlcpy.c ../lib/strlcat.c ../lib/fko_util.c \
    ../lib/fko_util.h 

if WANT_C_UNIT_TESTS
libfko_util_source_files += cunit_common.c cunit_common.h
endif

libfko_util_a_SOURCES    	= $(libfko_util_source_files)

AM_CPPFLAGS         		= $(GPGME_CFLAGS) -I $(top_srcdir)/common

EXTRA_DIST = common.h netinet_common.h cunit_common.h cunit_common.c
