# Elixir Bug: Modifying List During Enum.each Iteration

This example demonstrates a common error in Elixir when attempting to modify a list while iterating over it using `Enum.each`.  The issue stems from the immutability of Elixir data structures and the scope of variables within anonymous functions.

The provided code aims to remove the element `3` from the list. However, due to the way `Enum.each` works and the local variable scope, this doesn't achieve the desired result.  The solution demonstrates correct approaches using `Enum.filter` or `List.delete` in a proper way.