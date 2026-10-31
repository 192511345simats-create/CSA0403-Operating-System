# TASK 8 – Evaluate CPU States and Protection

## Objective

To understand CPU operating modes, protection mechanisms and the role of hardware support in protecting the operating system.

## Concept Details

This task explains how the operating system protects system resources using CPU modes and memory protection.

The major concepts covered are:

1. User Mode and Kernel Mode
2. Mode Bit
3. Privileged Instructions
4. Interrupts and Traps
5. Timer Interrupts
6. Memory Management Unit (MMU)
7. Memory Protection
8. Polling and Interrupt-Driven I/O

## Important Concepts

| Concept                 | Description                                                                |
| ----------------------- | -------------------------------------------------------------------------- |
| User Mode               | Mode in which normal application programs execute                          |
| Kernel Mode             | Mode in which the operating system performs privileged operations          |
| Mode Bit                | Indicates the current CPU execution mode                                   |
| Privileged Instructions | Instructions that can only be executed in kernel mode                      |
| Interrupt               | Signal that requests CPU attention                                         |
| Trap                    | Software-generated interrupt used for system calls or exception handling   |
| Timer Interrupt         | Ensures that the operating system regains CPU control periodically         |
| MMU                     | Hardware component that supports memory protection and address translation |

## Polling vs Interrupts

| Polling                             | Interrupt-Driven I/O                              |
| ----------------------------------- | ------------------------------------------------- |
| CPU repeatedly checks device status | Device signals the CPU when attention is required |
| Can waste CPU time                  | Reduces unnecessary CPU checking                  |
| Simple implementation               | Requires interrupt-handling support               |

## Software Requirements

* Operating System: Ubuntu 18.04.3
* Topic: Operating Systems
* Assignment: CSA04 – CO1

## Files Included

| File Name           | Description                                                         |
| ------------------- | ------------------------------------------------------------------- |
| `README.md`         | Task description and concept summary                                |
| `Task08_Answer.pdf` | Detailed theoretical explanation                                    |
| `output.png`        | Screenshot of relevant diagrams or assignment evidence, if required |

## Result

The concepts of CPU execution modes, hardware protection, memory protection and interrupt handling were studied.

## Conclusion

Thus, CPU states and protection mechanisms were evaluated to understand how an operating system protects its resources and ensures secure execution of processes.
