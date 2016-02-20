# Lab 6

## Exercise 1

To take into account multiple CPUs all generating time interrupts, I introduced an array of tick counts, where the index in the array is the number of the CPU that generated the time interrupt. To associate tick counts with CPU numbers, I changed some of the methods in `time.c` to accept the CPU number as an argument.

## Exercise 2 & 3

Read/skimmed the relevant chapters of the Intel manual. Added the network vendor and product ID constants to the `e1000.h` file and added a function to attach and enable the network card. I chose to keep the network attach function in the `pci.c` file because that is where the bridge attach function also lives.