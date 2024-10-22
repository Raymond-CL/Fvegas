# Fvegas
VEGAS multi-dimensional integration in Fortran

## original
This is the original code by G. Peter Lepage CLNS-80/447 March, 1980
```shell
gfortran -std=legacy -o original.exe vegas.f xvegas.f
```
note: 'ncall' was modified from 5000 to 4999 so that the output is similar to the one in the paper.