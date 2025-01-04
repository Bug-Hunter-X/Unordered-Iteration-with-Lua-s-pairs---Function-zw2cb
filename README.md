This repository demonstrates a potential issue with Lua's pairs() function. The `bug.lua` file contains code that iterates over a nested table using pairs(). Because pairs() doesn't guarantee a specific iteration order, the output might vary across Lua implementations or even different executions on the same system.  The `bugSolution.lua` file shows a way to address this by explicitly ordering the iteration if the sequence matters.