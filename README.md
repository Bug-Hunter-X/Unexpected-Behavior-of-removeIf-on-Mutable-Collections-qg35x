# Unexpected Behavior of removeIf on Mutable Collections in Kotlin

This example demonstrates a common unexpected behavior of the `removeIf` function in Kotlin when used with mutable collections like `MutableList` and `MutableSet`.  Instead of returning a new modified collection, `removeIf` directly modifies the original collection.

**Problem:** Developers often assume `removeIf` returns a new collection, leading to potential bugs when they expect the original collection to remain unchanged.

**Solution:** To maintain the original collection, explicitly create a copy before using `removeIf`.

This repo contains Kotlin code demonstrating the issue and its solution.