# Common Assembly Language Errors: Memory Access and Integer Overflow

This repository demonstrates two common errors in assembly language programming:

1. **Memory Access Violations:** Accessing memory locations outside of the allocated address space. This usually leads to segmentation faults.
2. **Integer Overflow:**  The result of an arithmetic operation exceeds the maximum value representable in the data type. This can cause unpredictable results.

The `bug.asm` file contains code demonstrating these errors. The `bugSolution.asm` provides corrected versions with improved error handling.

## How to Reproduce the Bug

1. Assemble and link `bug.asm`.
2. Run the resulting executable.
3. Observe the segmentation fault or unexpected behavior due to integer overflow.

## Bug Solution

The `bugSolution.asm` file shows how to mitigate these errors by:

* **Proper Memory Address Validation:** Before accessing memory, verify that the pointer is valid and points to a writable location.
* **Integer Overflow Prevention:** Using larger data types or checking for potential overflow conditions before performing operations. 

This example highlights the importance of careful memory management and error handling in low-level programming languages like assembly language.