#
#
AC_INIT([Xfwm4CompositeEditor],[0.2.1],[PROJ],[Xfwm4CompositeEditor])

AC_CONFIG_HEADER([config.h])
AC_PROG_CXX

AM_INIT_AUTOMAKE

AC_PROG_CC
AC_HEADER_STDC

AC_SUBST(CFLAGS)
AC_SUBST(CPPFLAGS)
AC_SUBST(LDFLAGS)
AM_PROG_CC_C_O

CXXFLAGS=-Wall
AC_SUBST(CXXFLAGS)

CFLAGS=-Wall
AC_SUBST(CFLAGS)

GTK_MODULES="gtk+-2.0 >= 2.24.0"
PKG_CHECK_MODULES(GTK, $GTK_MODULES)
AC_SUBST(GTK_CFLAGS)
AC_SUBST(GTK_LIBS)

XFCE4UI_MODULES="libxfce4ui-1 >= 4.8.0"
PKG_CHECK_MODULES(XFCE4UI, $XFCE4UI_MODULES,AC_DEFINE([GOT_LIBXFCEUI], [], [Description]),echo "INFORMATION ... Not using Xfce4 dialog header")

AC_SUBST([XFCE4UI_CFLAGS])
AC_SUBST([XFCE4UI_LIBS])

XFCONF_MODULES="libxfconf-0 >= 4.8.1"
PKG_CHECK_MODULES(XFCONF, $XFCONF_MODULES)
AC_SUBST(XFCONF_CFLAGS)
AC_SUBST(XFCONF_LIBS)

AC_OUTPUT(Makefile Xfwm4CompositeEditor/app/Makefile)

