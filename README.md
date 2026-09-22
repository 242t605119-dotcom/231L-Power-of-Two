# LeetCode 231 - Power of Two

## Problem

Given an integer `n`, return `true` if it is a power of two. Otherwise, return `false`.

An integer is a power of two if there exists an integer `x` such that:

```text
n = 2^x
```

## Example

### Input

```text
n = 16
```

### Output

```text
true
```

### Example 2

```text
n = 3
```

Output:

```text
false
```

### Example 3

```text
n = 1
```

Output:

```text
true
```

## Approach

A positive power of two has exactly one `1` bit in its binary representation.

For example:

```text
1  = 0001
2  = 0010
4  = 0100
8  = 1000
16 = 10000
```

For a power of two, `n & (n - 1)` is always `0`.

We also check that `n` is positive.

## Algorithm

1. Check if `n` is greater than `0`.
2. Calculate `n & (n - 1)`.
3. If the result is `0`, `n` is a power of two.
4. Otherwise, it is not a power of two.

## Complexity

* Time Complexity: `O(1)`
* Space Complexity: `O(1)`

## Language

Python

## LeetCode

Problem: 231 - Power of Two

## Author

**T.Nandhini**
