#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.68])
AC_INIT([libsiren], [1.0], [https://github.com/kakaroto/libsiren/issues])
AC_CONFIG_SRCDIR([siren7.h])
AC_CONFIG_HEADERS([config.h])
AM_INIT_AUTOMAKE([-Wall])

# Set the libtool C/A/R version info
#    If the source code was changed, but there were no interface changes:
#      Increment REVISION.
#    If there was a compatible interface change:
#      Increment CURRENT and AGE. Set REVISION to 0
#    If there was an incompatible interface change:
#      Increment CURRENT. Set AGE and REVISION to 0
LIBSIREN_CURRENT=0
LIBSIREN_REVISION=0
LIBSIREN_AGE=0
LIBSIREN_LIBVERSION=${LIBSIREN_CURRENT}:${LIBSIREN_REVISION}:${LIBSIREN_AGE}
LIBSIREN_LT_LDFLAGS="-version-info ${LIBSIREN_LIBVERSION} -no-undefined"
AC_SUBST(LIBSIREN_LT_LDFLAGS)

AM_SILENT_RULES([yes])

# Checks for programs.
AC_PROG_CC
AC_PROG_LIBTOOL

# Checks for libraries.

# Checks for header files.
AC_CHECK_HEADERS([stdlib.h string.h])

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.
AC_FUNC_MALLOC
AC_CHECK_LIBM
AC_CHECK_FUNCS([memset pow sqrt])
AC_SUBST(LIBM)

AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_FILES([
Makefile
libsiren.pc
])
AC_OUTPUT
