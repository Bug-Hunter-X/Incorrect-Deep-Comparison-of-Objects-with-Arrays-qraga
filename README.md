# Incorrect Deep Comparison of Objects with Arrays

This repository demonstrates a bug in a JavaScript function designed for deep comparison of objects. The function incorrectly handles array comparisons, returning `false` even when arrays are structurally identical.

## Bug Description
The `foo` function aims to perform a recursive deep comparison of two objects. However, it fails to correctly compare arrays, resulting in inaccurate comparison results.

## How to Reproduce
1. Clone this repository.
2. Run `node bug.js`.
3. Observe the incorrect output for the comparison involving objects with arrays (`obj5` and `obj6`).

## Solution
The solution involves adding a check to handle arrays and use strict equality (`===`) for comparing array elements.