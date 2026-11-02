# Q1 – Linking, Loading and Address Binding

**Aim:** To implement and compare static linking, dynamic linking and runtime loading using C.

**Requirements:**

* OS: Ubuntu 18.04.3
* Language: C
* Compiler: GCC

**Files:**

* `bank.c`
* `encryption.c`
* `encryption.h`
* `runtime_load.c`

**Compilation and Execution:**

```bash
gcc -c encryption.c -o encryption.o
ar rcs libencryption.a encryption.o
gcc bank.c ./libencryption.a -o bank_static
./bank_static
```

**Dynamic Linking:**

```bash
gcc -fPIC -c encryption.c -o encryption.o
gcc -shared -o libencryption.so encryption.o
gcc bank.c -L. -Wl,-rpath,'$ORIGIN' -lencryption -o bank_dynamic
./bank_dynamic
```

**Check Libraries and Size:**

```bash
ls -lh bank_static bank_dynamic
ldd bank_dynamic
```

**Runtime Loading:**

```bash
gcc runtime_load.c -o runtime_load -ldl
./runtime_load
```

**Result:** Static linking, dynamic linking and runtime loading were implemented and compared.

**Conclusion:** Dynamic linking allows shared libraries to be updated without recompiling the main application, provided compatibility is maintained.
