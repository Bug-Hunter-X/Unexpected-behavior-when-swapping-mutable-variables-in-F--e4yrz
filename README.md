# Unexpected Behavior When Swapping Mutable Variables in F#

This example demonstrates an unexpected behavior that can occur when swapping mutable variables in F#.  Due to the pass-by-reference nature of mutable variables, the swap function directly modifies the original variables, leading to incorrect results.

The file `bug.fs` contains the buggy code, and `bugSolution.fs` provides a corrected version.

## How to reproduce the bug:
1. Compile and run `bug.fs`.
2. Observe the incorrect output.

## Solution:
The solution in `bugSolution.fs` shows how to correctly swap variables using tuples to avoid the pass-by-reference issue.