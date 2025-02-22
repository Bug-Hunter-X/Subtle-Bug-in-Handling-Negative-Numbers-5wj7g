# Julia Bug: Unexpected Negative Result

This repository demonstrates a subtle bug in a Julia function that incorrectly handles negative numbers. The function intends to square its input and return a positive value, but it inadvertently returns a negative value for negative inputs.

The `bug.jl` file contains the buggy code, and `bugSolution.jl` provides a corrected version.

The problem stems from the way that the `-x^2` calculation is performed. This calculation effectively squares the input value, then negates the result.  The fix involves ensuring that the squaring operation returns a positive result before negating if required. 

This example highlights the importance of careful consideration when handling negative numbers in mathematical functions in Julia.