# Elixir Enum.reduce Bug: Missing Return

This repository demonstrates a subtle bug that can occur when using `Enum.reduce` in Elixir. The issue arises from a missing `return` statement in the anonymous function passed to `Enum.reduce`, which causes the function to behave unexpectedly. The code intends to sum only the even numbers in a list, but the omission of the `return` leads to incorrect results.

## Bug Description

The `bug.ex` file contains Elixir code using `Enum.reduce` to sum even numbers. Due to a missing `return` statement, the function doesn't always return the updated accumulator value, resulting in an incorrect sum.

## Solution

The `bugSolution.ex` file shows the corrected version where the `return` statement is explicitly included in the anonymous function, ensuring the accumulator is correctly updated in each iteration. This provides the expected sum of even numbers.

## How to reproduce

1. Clone this repository.
2. Navigate to the directory containing `bug.ex`.
3. Run the code using `elixir bug.ex` and observe the unexpected output.
4. Run the code in `bugSolution.ex` and observe the correct output.