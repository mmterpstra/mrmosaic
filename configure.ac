#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([mrmosaic], [0.1], [mail@example.com])
AC_CONFIG_SRCDIR([src/cnv_baf_data.c])

AC_CONFIG_FILES([Makefile
                 scripts/Makefile
                 src/Makefile])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CC
#note the src Makefile.am also has some compile flags enabled
#this is not best practice but thats why I put this comment here

# Checks for libraries.

# Checks for header files.
AC_CHECK_HEADERS([stdlib.h string.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_INT8_T

# Checks for library functions.
htslib_lib=ok
AC_CHECK_LIB(hts, hts_itr_next,  [], [htslib_lib=missing])
if test $htslib_lib != ok; then
  AC_MSG_ERROR([htslib library files not found])
fi

#AC_CONFIG_SUBDIRS([samtools-1.3])
AM_INIT_AUTOMAKE
AC_OUTPUT
