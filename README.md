# rosco_readtest
Some simple routines to test out the read performance of a SD Card on a rosco_m68k SBC

First run this on your PC/Mac with:
<code>
    cc test.c -o test 
    ./test
</code>
This creates and tests the test files. Next compile for the rosco_m68k use:
<code>
     ROSCO_M68K_DIR=~/rosco_m68k make EXTRA_CFLAGS=-DROSCO=1
</code>
Copy all the files across to the SD Card with:
<code>
    cp readtest* /Volumes/SDCARD
    cp rosco_readtest.bin /Volumes/SDCARD
</code>
Run rosco_readtest.bin on the rosco_m68k

To run on the Mac:
<code>
cc test.c -o test
./test
</code>
To run on the rosco_m68k:
<code>
ROSCO_M68K_DIR=~/rosco_m68k make EXTRA_CFLAGS=-DROSCO=1
</code>
