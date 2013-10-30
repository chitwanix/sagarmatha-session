bin_PROGRAMS = sagarmatha-session-quit
libexec_PROGRAMS = sagarmatha-session-check-accelerated sagarmatha-session-check-accelerated-helper

AM_CPPFLAGS =

AM_CFLAGS = $(WARN_CFLAGS)

sagarmatha_session_quit_SOURCES =			\
	sagarmatha-session-quit.c

sagarmatha_session_quit_CPPFLAGS =			\
	$(AM_CPPFLAGS)				\
	$(CINNAMON_SESSION_CFLAGS)			\
	$(DBUS_GLIB_CFLAGS)			\
	$(GCONF_FLAGS)				\
	-DLOCALE_DIR=\""$(datadir)/locale"\"	\
	$(DISABLE_DEPRECATED_CFLAGS)

sagarmatha_session_quit_LDADD =			\
	$(SM_LIBS)				\
	$(ICE_LIBS)				\
	$(CINNAMON_SESSION_LIBS)			\
	$(DBUS_GLIB_LIBS)			\
	$(GCONF_LIBS)

sagarmatha_session_check_accelerated_helper_SOURCES = 		\
	sagarmatha-session-check-accelerated-helper.c

sagarmatha_session_check_accelerated_helper_CPPFLAGS =	\
	-DPKGDATADIR=\""$(pkgdatadir)"\"		\
	$(GL_TEST_CFLAGS)

sagarmatha_session_check_accelerated_helper_LDADD = 		\
	$(GL_TEST_LIBS)				\
	$(X_LIBS)

sagarmatha_session_check_accelerated_SOURCES =       \
	sagarmatha-session-check-accelerated.c

sagarmatha_session_check_accelerated_CPPFLAGS =      \
	-DLIBEXECDIR=\""$(libexecdir)"\"	\
	$(AM_CPPFLAGS)			        \
	$(GTK3_CFLAGS)

sagarmatha_session_check_accelerated_LDADD =         \
	$(GTK3_LIBS)				\
	$(X_LIBS)

-include $(top_srcdir)/git.mk
