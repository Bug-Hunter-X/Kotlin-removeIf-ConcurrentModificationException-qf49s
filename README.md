# Kotlin removeIf ConcurrentModificationException

This repository demonstrates a subtle bug that can occur when using the `removeIf` function with iterators in Kotlin.
The example shows that when using `removeIf` on a mutable list or map, attempting to modify the collection while iterating over it using the `removeIf` method can throw a ConcurrentModificationException.  The fix involves creating a copy of the iterator or using a different approach entirely like filtering the collection and creating a new one.