dnl Process this file with autoconf to produce a configure script.
AC_PREREQ([2.69])
LT_PREREQ([2.4.2])
dnl
AC_INIT([bliss],[0.73],
	[tommi.junttila@aalto.fi],[bliss],
	[http://www.tcs.hut.fi/Software/bliss/])
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_SRCDIR([bliss_C.h])
AC_CONFIG_HEADERS([bliss_config.h])
AM_SILENT_RULES([yes])
AM_INIT_AUTOMAKE([foreign])
AM_MAINTAINER_MODE([])

AC_CANONICAL_HOST

dnl libtool
LT_INIT

dnl Checks for programs:
AC_PROG_CXX
AC_PROG_CC

dnl Checks for libraries:
dnl GNU MultiPrecision arithmetic library (GMP)
AM_PATH_GMP([6.1.0],[],[AC_MSG_ERROR(could not find required version of GMP)])

AC_CONFIG_FILES([
	include/Makefile
	include/bliss/Makefile
	Makefile
	])
AC_OUTPUT

dnl eof
