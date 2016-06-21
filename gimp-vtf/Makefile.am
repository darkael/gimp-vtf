## Process this file with automake to produce Makefile.in

bin_PROGRAMS = gimp-vtf

bindir = $(GIMP_LIBDIR)/plug-ins

gimp_vtf_SOURCES = \
	plugin-intl.h	\
	file-vtf.c \
	file-vtf.h \
	file-vtf-load.c \
	file-vtf-save.c

AM_CPPFLAGS = \
	-DLOCALEDIR=\""$(LOCALEDIR)"\"		\
	-DDATADIR=\""$(DATADIR)"\"

INCLUDES =\
	-I$(top_srcdir)		\
	@GIMP_CFLAGS@		\
	@VTFLIB_CFLAGS@		\
	-I$(includedir)

LDADD = $(GIMP_LIBS) -ltxc_dxtn $(VTFLIB_LIBS) -lm
