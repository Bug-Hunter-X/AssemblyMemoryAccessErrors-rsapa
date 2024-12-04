# Segmentation Fault in Assembly due to Invalid Memory Access

This repository contains an example of a segmentation fault in assembly code caused by attempting to access memory outside the program's valid address space. The code demonstrates a `mov` instruction that uses an invalid memory address calculation.

## Bug Description:

The assembly code includes a `mov` instruction that calculates the memory address using the `ebx`, `ecx` registers. If the calculated address falls outside the program's accessible memory, it results in a segmentation fault.

## Bug Solution:

The solution involves adding input validation to ensure that the values of `ebx` and `ecx` are within the allowed range. The solution also introduces error handling to prevent the program from crashing if an invalid memory access is attempted.
