# Silent Failure in Elixir Enum.each with throw

This example demonstrates a subtle issue when using `Enum.each` with `throw` in Elixir.  While `throw` stops the enumeration, it doesn't explicitly raise an exception outside the `Enum.each` function, potentially leading to unexpected behavior and silent failures.

The `bug.ex` file contains the problematic code. The `bugSolution.ex` file shows how to handle this issue properly using a `try...catch` block.

This is an uncommon error because it doesn't produce a typical error message.  Instead, the program might seem to end prematurely without any clear indication of the problem.
