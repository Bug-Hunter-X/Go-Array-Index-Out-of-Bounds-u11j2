# Go Array Index Out of Bounds

This repository demonstrates a common error in Go: accessing an array index that is out of bounds.  This often results in a runtime panic.

The `bug.go` file contains the erroneous code.  The `bugSolution.go` file provides the corrected version.

## Bug Description
The provided code iterates beyond the valid indices of the array, causing a runtime panic.  The loop counter goes from 0 to 9 while the array only has indices 0 through 4.

## Solution
The solution involves ensuring that the loop does not try to access indices that are greater than or equal to the length of the array.