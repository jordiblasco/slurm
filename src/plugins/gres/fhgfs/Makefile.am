# Makefile for gres/mic plugin

AUTOMAKE_OPTIONS = foreign

PLUGIN_FLAGS = -module -avoid-version --export-dynamic

AM_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/src/common $(HWLOC_CPPFLAGS)

pkglib_LTLIBRARIES = gres_fhgfs.la

# Gres MIC plugin.
gres_fhgfs_la_SOURCES = gres_fhgfs.c
gres_fhgfs_la_LDFLAGS = $(SO_LDFLAGS) $(PLUGIN_FLAGS) $(HWLOC_LDFLAGS)
gres_fhgfs_la_LIBADD  = $(HWLOC_LIBS)
