# TASK 10 – Measure and Compare Operating System Performance

## Objective

To measure and compare the performance of system calls, process creation and thread creation in an operating system.

## Concept Details

This task evaluates the performance of different operating-system operations through practical experiments.

The major concepts covered are:

1. System-call performance
2. File-reading and writing operations
3. Buffer-size comparison
4. Process creation using `fork()`
5. Thread creation using `pthread_create()`
6. Process synchronization
7. Thread synchronization
8. Execution-time measurement

## Programs Included

| Program     | Description                                                    |
| ----------- | -------------------------------------------------------------- |
| `copy.c`    | Measures file-copying performance using different buffer sizes |
| `process.c` | Creates and measures multiple processes                        |
| `thread.c`  | Creates and measures multiple threads                          |

## Software Requirements

* Operating System: Ubuntu 18.04.3
* Programming Language: C
* Compiler: GCC
* Library: POSIX Threads (pthread)
* Tool: strace
* Time Measurement: Linux time command

## Compilation and Execution

### 1. File Copy Program

Compile:

```bash
gcc copy.c -o copy
```

Execute:

```bash
./copy
```

Measure system calls:

```bash
strace -c ./copy
```

Measure execution time:

```bash
time ./copy
```

### 2. Process Creation Program

Compile:

```bash
gcc process.c -o process
```

Execute:

```bash
time ./process
```

### 3. Thread Creation Program

Compile:

```bash
gcc thread.c -o thread -pthread
```

Execute:

```bash
time ./thread
```

## Performance Comparison

The experiments compare:

* Number of read and write system calls.
* Effect of buffer size on file-copying performance.
* Time required for process creation.
* Time required for thread creation.
* Resource usage and execution overhead.

## Files Included

| File Name                 | Description                                 |
| ------------------------- | ------------------------------------------- |
| `README.md`               | Task description and execution instructions |
| `Task10_Answer.pdf`       | Detailed theoretical explanation            |
| `copy.c`                  | File-copying performance program            |
| `process.c`               | Process creation program                    |
| `thread.c`                | Thread creation program                     |
| `output.png`              | Actual execution screenshots                |
| `strace_output.txt`       | Actual system-call statistics               |
| `performance_results.txt` | Actual measured performance results         |

## Result

The performance of system calls, process creation and thread creation is measured and compared. The results help understand the overhead and resource requirements of different operating-system operations.

**Note:** Actual execution times and performance measurements must be recorded from the Linux environment. Do not use assumed timings as experimental results.

## Conclusion

Thus, operating-system performance was measured and compared through file operations, process creation and thread creation experiments.
