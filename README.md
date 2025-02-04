# Lua `pairs` Iteration Order Inconsistency

This repository demonstrates a potential issue with the `pairs` iterator in Lua. The order of iteration might not be consistent across different Lua versions or implementations.  This inconsistency becomes particularly relevant when performing recursive operations on tables, as demonstrated in the `bug.lua` file.

The `bugSolution.lua` file offers a potential workaround to address this issue, ensuring more predictable behavior.  Note that this workaround might have performance implications.

## Reproducing the Issue
1. Clone this repository.
2. Run `bug.lua` using your preferred Lua interpreter.
3. Observe the output. The order of key-value pairs printed might differ across different Lua interpreters or versions.

## Solution
The `bugSolution.lua` file demonstrates a potential approach to mitigate the iteration order unpredictability.  Consider the trade-off between consistency and performance before implementing this solution in production code.