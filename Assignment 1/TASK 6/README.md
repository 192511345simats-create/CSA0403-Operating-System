# TASK 6 – Evaluate the Cost of System Calls

## Objective

To understand the cost of system calls and evaluate how buffer size affects file-reading performance and the number of system calls.

## Program Details

The C program `copy.c` demonstrates file copying using the `read()` and `write()` system calls.

It performs the following operations:

1. Opens the input file using `open()`.
2. Reads data using `read()`.
3. Writes data into the output file using `write()`.
4. Counts the read system calls.
5. Closes the files using `close()`.

## Files Included

| File Name           | Description                                  |
| ------------------- | -------------------------------------------- |
| `copy.c`            | C program for file copying                   |
| `input.txt`         | Input file containing sample data            |
| `output.txt`        | File created after copying                   |
| `Task06_Answer.pdf` | Detailed theoretical explanation             |
| `output.png`        | Screenshot of program execution              |
| `strace_output.txt` | System-call statistics obtained using strace |

## Software Requirements

* Operating System: Ubuntu 18.04.3
* Programming Language: C
* Compiler: GCC
* System-call tracing tool: strace

## Compilation

```bash
gcc copy.c -o copy
```

## Execution

```bash
./copy
```

## System Call Analysis

To display system-call statistics:

```bash
strace -c ./copy
```

To display only read and write system calls:

```bash
strace -c -e trace=read,write ./copy
```

To measure execution time:

```bash
time ./copy
```

## Result

The program demonstrates file copying using system calls. The experiment explains how buffer size affects the number of read operations and how buffering can reduce system-call overhead.

**Note:** Actual execution results and system-call statistics should be added after running the program.

## Conclusion

Thus, the cost of system calls was studied, and the effect of buffer size on file-processing performance was evaluated.
