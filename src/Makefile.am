## Process this file with automake to produce Makefile.in

## Created by Anjuta


uidir = $(pkgdatadir)/ui
ui_DATA = dnd_charsheet.ui


AM_CPPFLAGS = \
	-DPACKAGE_LOCALE_DIR=\""$(localedir)"\" \
	-DPACKAGE_SRC_DIR=\""$(srcdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(pkgdatadir)"\" \
	$(DND_CHARSHEET_CFLAGS)

AM_CFLAGS =\
	 -Wall\
	 -g

bin_PROGRAMS = dnd_charsheet

dnd_charsheet_SOURCES = \
	dnd_charsheet.vala config.vapi

dnd_charsheet_VALAFLAGS =  \
	--pkg gtk+-3.0

dnd_charsheet_LDFLAGS = \
	-Wl,--export-dynamic

dnd_charsheet_LDADD = $(DND_CHARSHEET_LIBS)


EXTRA_DIST = $(ui_DATA)

# Remove ui directory on uninstall
uninstall-local:
	-rm -r $(uidir)
	-rm -r $(pkgdatadir)

