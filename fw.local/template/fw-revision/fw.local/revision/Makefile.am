SUBDIRS = NAME

fwfwrevisionfwlocalrevisiondir = $(prefix)/share/fw/template/fw-revision/fw.local/revision

dist_fwfwrevisionfwlocalrevision_DATA = 	\
  Makefile_dot_am				\
  Makefile.am.local

install-data-hook:
	find "$(DESTDIR)$(fwfwrevisionfwlocalrevisiondir)" -type f | xargs chmod -w

MAINTAINERCLEANFILES = 				\
  Makefile.in

include $(top_srcdir)/fw/build/automake/gnu-make-check.am
