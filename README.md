# C++ Off-by-One Error in Vector Iteration

This repository demonstrates a common off-by-one error in C++ when iterating through a `std::vector`.  The error occurs because the loop condition checks `i <= vec.size()`, which attempts to access an element beyond the valid range of the vector (vectors are zero-indexed).  The solution corrects the loop condition to avoid this error.

## Bug
The `bug.cpp` file contains the buggy code.  It attempts to iterate through a vector using an incorrect loop condition, leading to an out-of-bounds access.

## Solution
The `bugSolution.cpp` file provides the corrected code.  The loop condition is changed to `i < vec.size()` to ensure that only valid indices are accessed.

This example highlights the importance of careful attention to loop bounds when working with dynamic arrays and vectors in C++.