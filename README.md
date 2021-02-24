# Build-Your-Own-Lisp

This is an implementation of a minimal, Lisp-like language as described in the book [Build Your Own Lisp](http://www.buildyourownlisp.com/). 

## Dependencies

The (mpc)[https://github.com/orangeduck/mpc] library is currently required for parsing the language's grammar. If building from source, mpc.h and mpc.c should be present in the directory.

## Building

A pre-compiled binary is available under releases, however, if you would like to compile from source, you can do so using GCC.

`gcc -std=c99 -Wall lispy.c mpc.c -g -ledit -lm -o lispy`

The standard library adds several useful functions, and can be loaded with the command `load "stdlib.lspy"`.