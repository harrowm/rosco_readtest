# rosco_readtest
Some simple routines to test out the read performance of a SD Card on a rosco_m68k SBC

To run on the Mac:
<code>
cc test.c -o test
./test
</code>
To run on the rosco_m68k:
<code>
ROSCO_M68K_DIR=~/rosco_m68k make EXTRA_CFLAGS=-DROSCO=1
</code>
