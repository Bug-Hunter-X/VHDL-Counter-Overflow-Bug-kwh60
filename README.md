# VHDL Counter with Overflow Handling

This repository demonstrates a common VHDL coding error related to counter overflow and presents a corrected version with improved overflow handling.

## Bug Description

The original `counter.vhdl` file contains a simple counter.  However, it lacks explicit handling for potential overflow conditions.  While the code appears to work correctly for typical scenarios, edge cases (such as unexpected clock glitches) or long simulations might expose the bug. If the counter exceeds its maximum value (15), it might not reset reliably, leading to unexpected outputs or simulation errors. 

## Solution

The corrected code, `counter_solution.vhdl` explicitly handles the counter exceeding its maximum value.  This solution ensures that the counter reliably resets when reaching the limit, leading to robust and predictable behavior.

## How to Use

1.  Simulate `counter_bug.vhdl` to observe the potential overflow issue (consider adding some unusual clock inputs).
2.  Compare the results with the behavior of `counter_solution.vhdl` to see how the issue has been resolved.

This example highlights the importance of robust error handling in VHDL code, especially in critical timing applications.