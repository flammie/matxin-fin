AC_PREREQ(2.52)

AC_INIT([matxin-fin], [0.0.0], [flammie@iki.fi])
AM_INIT_AUTOMAKE(no-define)
AC_PROG_LN_S
AC_PROG_AWK

AC_PATH_PROG(CGCOMP, cg-comp, no)
AS_IF([test x$ac_cv_path_CGCOMP = xno],
      [AC_MSG_ERROR([You do not have cg-comp installed.])])
AS_IF([test x$ac_cv_path_CGPROC = xno],
      [AC_MSG_ERROR([You do not have cg-comp installed.])])

AC_OUTPUT([Makefile matxin-fin.pc])
