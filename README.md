# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over arrays.  The `BuggyArray.java` file contains the erroneous code, which attempts to access an array element beyond its bounds.  The `CorrectedArray.java` file provides the corrected version.

## Bug Description:

The bug lies in the for loop's condition `i <= arr.length`.  Array indices in Java are zero-based, so the valid indices for an array of length n are 0 to n-1.  The loop iterates one element too far, causing an `ArrayIndexOutOfBoundsException`.

## Solution:

The solution is to change the loop condition to `i < arr.length`, ensuring the loop terminates before accessing an invalid index.