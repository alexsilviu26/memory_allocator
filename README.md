# Memory Allocator – C Project

Custom dynamic memory allocator implemented in **C**, designed to simulate the internal behavior of standard memory management functions such as `malloc`, `free`, `calloc`, and `realloc`.

The allocator manages heap memory manually using **low-level Linux system calls** such as `sbrk`, `mmap`, and `munmap`.

---

# Overview

This project implements a simplified **memory management system** similar to the one used internally by the C standard library.

Instead of relying on the operating system allocator, the program:

- manually allocates heap memory
- manages memory blocks
- tracks free and allocated memory
- performs block splitting and coalescing
- handles large allocations using memory mapping

The implementation demonstrates how dynamic memory allocation works at a low level.

---

# Implemented Functions

The allocator implements custom versions of the following functions:

- `os_malloc()` – allocates memory
- `os_free()` – frees allocated memory
- `os_calloc()` – allocates zero-initialized memory
- `os_realloc()` – resizes allocated memory

These functions mimic the behavior of their standard counterparts.

---
