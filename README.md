# myCSAPP

This repository is my working CS:APP study tree. It includes code based on the
official examples, but it is not only a copy of the provided source code. While
working through *Computer Systems: A Programmer's Perspective, 3rd Edition*, I
also add or change code here for my own questions, notes, tests, and ideas.

The directory map below follows the structure published on the official
CS:APP3e code examples page:

https://csapp.cs.cmu.edu/3e/code.html

It is intentionally high-level. Individual files are not documented here so
that examples can be added, removed, or changed without requiring a README
rewrite every time.

## Code structure

| Directory | Main association |
| --- | --- |
| `intro/` | Chapter 1, A Tour of Computer Systems |
| `data/` | Chapter 2, Representing and Manipulating Information |
| `asm/` | Chapter 3, Machine-Level Representation of Programs |
| `arch/` | Chapter 4, Processor Architecture examples and experiments |
| `opt/` | Chapter 5, Optimizing Program Performance |
| `perf/` | Chapter 5 support code for performance measurement experiments |
| `mem/` | Chapter 6, The Memory Hierarchy |
| `link/` | Chapter 7, Linking |
| `ecf/` | Chapter 8, Exceptional Control Flow |
| `error/` | System-level error-handling fragments used with later systems chapters |
| `vm/` | Chapter 9, Virtual Memory |
| `io/` | Chapter 10, System-Level I/O |
| `netp/` | Chapter 11, Network Programming |
| `conc/` | Chapter 12, Concurrent Programming |
| `include/` | Shared CS:APP headers used across multiple chapters |
| `src/` | Shared CS:APP support implementation used across multiple chapters |
| `lib/` | Built support libraries used by the examples |

## Notes

- The official CS:APP3e page lists example source files and chapter references.
  This repository keeps the same broad chapter grouping, while also allowing my
  own changes, local notes, generated assembly, Makefiles, and experiments.
- Some directories contain more material than the official code-example list.
  Treat those as study additions or build artifacts unless a subdirectory README
  says otherwise.
- When adding new code, prefer placing it under the chapter directory that best
  matches the concept being studied.
