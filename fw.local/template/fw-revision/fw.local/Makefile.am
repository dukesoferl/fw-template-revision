SUBDIRS = revision

fwfwrevisionfwlocaldir = $(prefix)/share/fw/template/fw-revision/fw.local

dist_fwfwrevisionfwlocal_DATA = 	\
  Makefile_dot_am			\
  Makefile.am.local

install-data-hook:
	find "$(DESTDIR)$(fwfwrevisionfwlocaldir)" -type f | xargs chmod -w

MAINTAINERCLEANFILES = 			\
  Makefile.in

include $(top_srcdir)/fw/build/automake/gnu-make-check.am
