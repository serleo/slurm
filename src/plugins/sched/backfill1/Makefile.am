# Makefile for backfill scheduler plugin

AUTOMAKE_OPTIONS = foreign

AM_CXXFLAGS = -fexceptions

PLUGIN_FLAGS = -module -avoid-version --export-dynamic

AM_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/src/common -I/usr/local/include

pkglib_LTLIBRARIES = sched_backfill1.la

sched_backfill1_la_SOURCES = backfill_wrapper.c	\
			backfill.c	\
			backfill.h
sched_backfill1_la_LDFLAGS = $(SO_LDFLAGS) $(PLUGIN_FLAGS) -L/usr/local/lib -lconfig
