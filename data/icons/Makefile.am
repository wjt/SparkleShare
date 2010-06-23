theme = hicolor
themedir = $(pkgdatadir)/icons/$(theme)
hicolordir = $(DESTDIR)$(datadir)/icons/hicolor

theme_icons =						\
	animations,process-syncing-sparkleshare-24.png	\
	animations,process-working-48.png		\
	emblems,emblem-synced-22.png			\
	emblems,emblem-synced-24.png			\
	emblems,emblem-sync-error-22.png		\
	emblems,emblem-sync-error-24.png		\
	emblems,emblem-syncing-22.png			\
	emblems,emblem-syncing-24.png			\
	places,fedorahosted-16.png			\
	places,folder-16.png				\
	places,folder-22.png				\
	places,folder-24.png				\
	places,folder-256.png				\
	places,folder-32.png				\
	places,folder-48.png				\
	places,folder-sparkleshare-16.png		\
	places,folder-sparkleshare-22.png		\
	places,folder-sparkleshare-24.png		\
	places,folder-sparkleshare-256.png		\
	places,folder-sparkleshare-32.png		\
	places,folder-sparkleshare-48.png		\
	places,github-16.png				\
	places,gitorious-16.png				\
	places,gnome-16.png				\
	status,avatar-default-16.png			\
	status,avatar-default-22.png			\
	status,avatar-default-24.png			\
	status,avatar-default-32.png			\
	status,avatar-default-48.png			\
	status,document-added-16.png			\
	status,document-edited-16.png			\
	status,document-moved-16.png			\
	status,document-removed-16.png			\
	status,folder-synced-22.png			\
	status,folder-synced-24.png			\
	status,folder-sync-error-22.png			\
	status,folder-sync-error-24.png			\
	status,folder-syncing-22.png			\
	status,folder-syncing-24.png

install_icon_exec = $(top_srcdir)/icon-theme-installer \
	-t "$(theme)" \
	-s "$(srcdir)" \
	-d "x$(DESTDIR)" \
	-b "$(themedir)" \
	-m "$(mkinstalldirs)" \
	-x "$(INSTALL_DATA)"

install-data-local:
	@-$(install_icon_exec) -i $(theme_icons)

uninstall-hook:
	@-$(install_icon_exec) -u $(theme_icons)

MAINTAINERCLEANFILES = Makefile.in
EXTRA_DIST = $(wildcard *.png *.svg)