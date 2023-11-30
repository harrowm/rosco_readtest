# rosco_readtest
Some simple routines to test out the read performance of a SD Card on a rosco_m68k SBC

First run this on your PC/Mac with:

```shell
    cc test.c -o test 
    ./test
```

This creates and tests the test files. Next compile for the rosco_m68k use:

```shell
     ROSCO_M68K_DIR=~/rosco_m68k make EXTRA_CFLAGS=-DROSCO=1
```

Copy all the files across to the SD Card with:

```shell
    cp readtest* /Volumes/SDCARD
    cp rosco_readtest.bin /Volumes/SDCARD
```

Run rosco_readtest.bin on the rosco_m68k

