# TASK 7 – Evaluate Process Control System Calls

## Objective

To understand and evaluate process control system calls such as `fork()`, `exec()` and `waitpid()` in the Linux operating system.

## Program Details

The C program demonstrates process creation, execution and termination using process control system calls.

It performs the following operations:

1. Creates a child process using `fork()`.
2. Executes a command in the child process using `execlp()`.
3. Waits for the child process to complete using `waitpid()`.
4. Retrieves and displays the child process exit status.
5. Demonstrates process termination using `_exit()`.

## Files Included

| File Name           | Description                                          |
| ------------------- | ---------------------------------------------------- |
| `process.c`         | C program demonstrating process control system calls |
| `Task07_Answer.pdf` | Detailed theoretical explanation                     |
| `output.png`        | Screenshot of actual program execution               |
| `README.md`         | Program description and execution instructions       |

## Software Requirements

* Operating System: Ubuntu 18.04.3
* Programming Language: C
* Compiler: GCC

## Compilation

```bash
gcc process.c -o process
```

## Execution

```bash
./process
```

## System Calls Used

| System Call | Purpose                                       |
| ----------- | --------------------------------------------- |
| `fork()`    | Creates a new child process                   |
| `execlp()`  | Replaces the child process with a new program |
| `waitpid()` | Waits for a specific child process            |
| `_exit()`   | Terminates a process immediately              |

## Expected Output

```text
shell: running job 1
42
job 1 exit status 0
shell: running job 2
job 2 exit status 3
```

*The output may vary slightly depending on the execution environment.*

## Result

The program demonstrates process creation, execution, synchronization and termination using Linux process control system calls.

## Conclusion

Thus, process control system calls were studied and implemented using C programming in the Linux operating system.
