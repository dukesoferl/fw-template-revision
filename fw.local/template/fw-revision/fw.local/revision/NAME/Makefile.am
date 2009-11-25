fwfwrevisionfwlocalnamedir = $(prefix)/share/fw/template/fw-revision/fw.local/revision/NAME

dist_fwfwrevisionfwlocalname_DATA = 		\
  Makefile.am.local				\
  Makefile_dot_am

dist_fwfwrevisionfwlocalname_SCRIPTS =		\
  add-dir					\
  add-files					\
  check-for-tag					\
  check-up-to-date				\
  detect					\
  ignore-files					\
  init						\
  init-fw-pkgin-config				\
  remove-files					\
  tag

noinst_DATA =					\
  $(dist_fwfwrevisionfwlocalname_SCRIPTS:%=.%.script_ok)

install-data-hook:
	find "$(DESTDIR)$(fwfwrevisionfwlocalnamedir)" -type f | xargs chmod -w

CLEANFILES =					\
  $(wildcard .*.script_ok)

MAINTAINERCLEANFILES = 				\
  Makefile.in

include $(top_srcdir)/fw/build/automake/check-shell.am
include $(top_srcdir)/fw/build/automake/gnu-make-check.am
