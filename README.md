# Fvegas
VEGAS multi-dimensional integration in Fortran

## `original`
This is the original code by G. Peter Lepage CLNS-80/447 March, 1980
compile with the following:
```shell
gfortran -std=legacy -o original.exe vegas.f xvegas.f
```
note: 'ncall' was modified from 5000 to 4999 so that the output is similar to the one in the paper.

## `nf_f77`
This is the numerical recipe version written in Fortran 77 standard
compile with the following:
```shell
gfortran -std=legacy -fdefault-real-8 -o nr77.exe ran2.for rebin.fo vegas.for xvegas.for
```
note: the `-fdefault-real-8` flag might be needed to get rid of a warning message from denormal numbers.