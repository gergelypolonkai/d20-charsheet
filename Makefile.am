## Process this file with automake to produce Makefile.in
## Created by Anjuta

SUBDIRS = src 

dnd_charsheetdocdir = ${prefix}/doc/dnd_charsheet
dnd_charsheetdoc_DATA = \
	README\
	COPYING\
	AUTHORS\
	ChangeLog\
	INSTALL\
	NEWS


EXTRA_DIST = $(dnd_charsheetdoc_DATA)


# Remove doc directory on uninstall
uninstall-local:
	-rm -r $(dnd_charsheetdocdir)
