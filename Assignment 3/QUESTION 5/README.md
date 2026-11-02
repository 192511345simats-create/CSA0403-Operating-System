# Q5 – Page-Replacement Techniques

**Aim:** To implement and compare FIFO, LRU and Optimal page-replacement algorithms.

**Requirements:**

* OS: Ubuntu 18.04.3
* Language: C
* Compiler: GCC

**File:**

* `page_replacement.c`

**Compilation and Execution:**

```bash
gcc page_replacement.c -o page_replacement
./page_replacement
```

**Concepts Covered:**

* FIFO
* LRU
* Optimal Page Replacement
* Page Faults
* Belady's Anomaly
* Clock Algorithm

**Result:** FIFO, LRU and Optimal algorithms were implemented and compared using page-fault counts.

**Conclusion:** LRU provides better page replacement than FIFO, while Optimal produces the minimum page faults.
