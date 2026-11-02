# Q6 – Disk Management

**Aim:** To study disk management, RAID configurations, partitioning and swap-space management.

**Requirements:**

* OS: Ubuntu 18.04.3
* Compiler: GCC

**Commands Used:**

```bash
lsblk
sudo fdisk -l
swapon --show
free -h
```

**Concepts Covered:**

* Disk Formatting
* Partitioning
* Boot Process
* Bad Block Handling
* RAID 0, 1, 5 and 10
* Swap Space

**Result:** Disk partitions, swap space and RAID configurations were studied.

**Conclusion:** RAID 10 is recommended for the hospital records server because it provides good performance and fault tolerance.
