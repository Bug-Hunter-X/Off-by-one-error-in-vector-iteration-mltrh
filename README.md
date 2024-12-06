# Off-by-One Error in C++ Vector Iteration

This repository demonstrates a common off-by-one error when iterating over a `std::vector` in C++.  The bug causes an out-of-bounds access, potentially leading to undefined behavior or crashes.

The `bug.cpp` file contains the erroneous code. The `bugSolution.cpp` file provides the corrected version.

## How to reproduce

1. Clone the repository.
2. Compile `bug.cpp` using a C++ compiler (e.g., g++).
3. Run the executable. Observe the error (likely a segmentation fault).
4. Compile and run `bugSolution.cpp` to see the corrected output.

## Lesson

Always double-check your loop conditions when iterating over containers.  Remember that the valid indices for a vector of size N are 0 to N-1.