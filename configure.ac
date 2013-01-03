AC_INIT([sirveillance], [0.1], [handdol@gmail.com])
AM_INIT_AUTOMAKE([foreign -Wall -Werror])
AC_PROG_CC
AC_PROG_CXX
AC_PROG_LIBTOOL

# Include necessary embedded library
m4_include([src/libev/libev.m4]) 

AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile src/Makefile src/libev/Makefile])
AC_OUTPUT
