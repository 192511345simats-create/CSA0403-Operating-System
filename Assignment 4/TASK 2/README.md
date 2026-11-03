# Task 2 – Storage for a Video-Surveillance Recorder

**Name:**
**Register Number:**
**Course:** CSA04 – Operating Systems
**Assignment:** CO4 – Assignment 4

## Objective

To analyse file operations and compare contiguous, linked and indexed allocation methods for a video-surveillance storage system.

## Concepts Used

* Sequential and direct access
* Contiguous allocation
* Linked allocation
* Indexed allocation
* Inode structure
* Free-space management
* First-fit allocation

## Implementation

A C program is implemented using first-fit contiguous allocation and indexed allocation to manage disk blocks.

## Compilation

```bash
gcc -std=c11 -Wall -Wextra task2.c -o task2
```

## Execution

```bash
./task2
```

## Result

The allocation methods are compared based on disk access, file growth, fragmentation and storage efficiency. The program demonstrates memory-block allocation using first-fit allocation.
