Startle Library
===============

Startle is a library of useful and efficient algorithms and facilities for developing C programs.

Library features include:

* Low overhead in-memory structured logging: deferred string formatting, indented with context, stored to a ring buffer, minimal overhead allowing use in release builds
* Macros: for common tasks such as iteration, bit/flag operations, intrusive lists
* Dispatch macros: Simulate overloaded functions for variable arguments
* Error handling
* Algorithms: Quicksort, binary search, string segments, simple mmap'ing, integer log, hash set
* Zero space overhead map: O(log(n)) insertion, O(log(n)^2) lookup, O(log(n)) in-place conversion to a sorted array for O(log(n)) lookup afterwards.

Makefile features include:

* Automatic dependency handling
* Integration with `makeheaders` to automatically generate and update headers for .c files
* Simple code generation: Collect macro-like annotations into lists for x-macros
  - Used for: Unit tests, handling commands and flags
  
Startle was originally developed as part of [PoprC](https://github.com/HackerFoo/poprc).
