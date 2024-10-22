# Fvegas
VEGAS multi-dimensional integration in Fortran
supplied with examples

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

## `nf_f90`
This is the numerical recipe version written in Fortran 90 standard
compile with the following:
```shell
gfortran -fno-strict-overflow -o nr90.exe nrtype.f90 nr.f90 nrutil.f90 ran_state.f90 ran1.f90 vegas.f90 xvegas.f90
```
note: the `-fno-strict-overflow` flag is needed for the RNG to work.