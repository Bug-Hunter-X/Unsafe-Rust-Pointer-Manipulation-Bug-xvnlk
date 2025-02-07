# Unsafe Rust Pointer Manipulation Bug

This repository demonstrates a common mistake when working with raw pointers in Rust. Modifying memory directly through a raw pointer can lead to unexpected behavior or memory corruption if not handled carefully.

The `bug.rs` file contains the buggy code, while `bugSolution.rs` provides a safer alternative using safe Rust techniques.

## Bug Description:

The code attempts to modify the first element of a vector using a raw pointer. This can lead to memory unsafety and undefined behavior if not handled carefully.

## Bug Solution:

The safe approach is to avoid direct manipulation of memory using raw pointers whenever possible. In this case, using standard vector methods like `v[0] = 10` is preferred.

This example highlights the importance of understanding memory management and using safe Rust practices to avoid common errors.