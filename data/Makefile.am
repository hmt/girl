SUBDIRS = pixmaps icons

@INTLTOOL_DESKTOP_RULE@

DESKTOP_IN_FILES= girl.desktop.in.in
DESKTOP_FILES= $(DESKTOP_IN_FILES:.desktop.in.in=.desktop)

desktopdir = $(datadir)/applications
desktop_DATA = $(DESKTOP_FILES)

@INTLTOOL_XML_RULE@
appdatadir = $(datadir)/appdata
appdata_in_files = girl.appdata.xml.in
appdata_DATA = $(appdata_in_files:.xml.in=.xml)

# gsettings_ENUM_NAMESPACE = org.gnome.girl
# gsettings_ENUM_FILES = $(top_srcdir)/src/eog-scroll-view.h	\
#                        $(top_srcdir)/src/eog-window.h
# gsettings_SCHEMAS = org.gnome.girl.gschema.xml

# @GSETTINGS_RULES@

# gsettingsconvertdir = $(datadir)/GConf/gsettings
# gsettingsconvert_DATA = eog.convert

# uidir = $(pkgdatadir)
# ui_DATA = \
# 	eog-toolbar.xml

# pkgconfigdir = $(libdir)/pkgconfig
# pkgconfig_DATA = girl.pc

EXTRA_DIST =			\
	$(DESKTOP_IN_FILES)	\
	$(appdata_in_files)

CLEANFILES = 			\
	$(appdata_DATA)

DISTCLEANFILES = 		\
        $(DESKTOP_FILES)
#        $(gsettings_SCHEMAS)

-include $(top_srcdir)/git.mk
