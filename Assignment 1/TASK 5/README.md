# TASK 5 – Examine System Calls

## Objective

To examine how programs obtain operating-system services through system calls.

## Contents

1. Categories of system calls:

   * Process control
   * File management
   * Device management
   * Information maintenance
   * Communication
   * Protection
2. Step-by-step explanation of the read() system call.
3. Parameter-passing methods:

   * Registers
   * Memory block
   * Stack
4. Explanation of how strace displays system calls made by a program.
5. Alternative concept and complexity analysis comparing C library functions (fopen, fread and fwrite) with direct system calls (open, read and write).

## Files

* Task05_Answer.pdf – Complete written answer and system-call explanation.
* read_example.c – C program used to demonstrate the read() system call.
* output.png – Screenshot of actual program execution and strace output.

## Conclusion

This task examines how system calls provide access to operating-system services and evaluates their performance using library buffering and direct system calls.
