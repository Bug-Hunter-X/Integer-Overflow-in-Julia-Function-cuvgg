# Integer Overflow Bug in Julia

This repository demonstrates a subtle integer overflow bug in a simple Julia function. The function is designed to square the input, handling positive, zero, and negative numbers differently. However, for sufficiently large negative integers, squaring leads to an overflow, resulting in unexpected output.

## Bug Description
The `myfunction` in `bug.jl` exhibits unexpected behavior when the input is a negative number that results in an integer overflow after squaring. This overflow manifests as an incorrect output, deviating from the expected result.

## Solution
The `bugSolution.jl` file presents a corrected version that addresses integer overflow by using floating-point numbers or explicitly handling potential overflows.

## How to Reproduce
1. Clone the repository.
2. Run `bug.jl` using Julia. Observe the unexpected result for certain negative input values.
3. Run `bugSolution.jl`. The corrected function should produce the expected output.