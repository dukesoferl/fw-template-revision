fwfwrevisiontestsdir = $(prefix)/share/fw/template/fw-revision/tests

dist_fwfwrevisiontests_SCRIPTS =	\
  test-revision

dist_fwfwrevisiontests_DATA = 		\
  Makefile.am.local			\
  Makefile_dot_am

install-data-hook:
	find "$(DESTDIR)$(fwfwrevisiontestsdir)" -type f | xargs chmod -w

noinst_DATA =				\
  $(dist_fwfwrevisiontests_SCRIPTS:%=.%.script_ok)

CLEANFILES =

MAINTAINERCLEANFILES = 			\
  Makefile.in

include $(top_srcdir)/fw/build/automake/check-shell.am
include $(top_srcdir)/fw/build/automake/gnu-make-check.am
