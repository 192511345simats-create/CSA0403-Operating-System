# Q7 – Memory-Management Plan

**Aim:** To design a memory-management plan for a smart factory edge device with 2 GB RAM.

**Requirements:**

* OS: Ubuntu 18.04.3
* Language: C
* Compiler: GCC

**File:**

* `memory_lock.c`

**Compilation and Execution:**

```bash
gcc memory_lock.c -o memory_lock
./memory_lock
```

**Concepts Covered:**

* Memory Allocation
* Paging
* Demand Paging
* Memory Locking (`mlock()`)
* Real-Time Tasks
* Page Faults

**Result:** Memory locking was implemented to protect the time-critical task from page faults caused by swapping.

**Conclusion:** Locked memory provides more predictable execution for real-time tasks while allowing other tasks to use available memory efficiently.
