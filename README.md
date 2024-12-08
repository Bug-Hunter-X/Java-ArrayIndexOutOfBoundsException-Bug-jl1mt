# Java ArrayIndexOutOfBoundsException Bug

This repository demonstrates a common Java programming error: the `ArrayIndexOutOfBoundsException`. The `BuggyArray.java` file contains code that attempts to access an array element beyond its valid index range, resulting in a runtime exception. The `FixedArray.java` file provides the corrected version.

## Bug Description
The `BuggyArray` code incorrectly uses `i <= arr.length` as the loop condition. Because arrays are zero-indexed, the valid indices are 0 to `arr.length - 1`. The condition should be `i < arr.length`.

## Solution
The `FixedArray` code corrects the loop condition to `i < arr.length`, preventing the `ArrayIndexOutOfBoundsException`.