# Implicit Type Coercion with Null Values in JavaScript

This repository demonstrates a common JavaScript bug related to implicit type coercion when null values are passed to a function. The bug arises from the function's implicit conversion of null values to 0, which may lead to unexpected behavior or incorrect results.

## Bug Description

The `foo` function does not explicitly handle null values. If null values are passed to `a` or `b`, JavaScript implicitly coerces null to 0, which may lead to unintended consequences.  This is especially problematic if the function's logic depends on distinguishing between null and 0.

## Bug Solution

The solution involves explicitly checking for null values using strict equality (`===`) and handling them appropriately. This prevents the implicit coercion of null to 0.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js`.
3. Run `bug.js` and observe the unexpected behavior. 
4. Run `bugSolution.js` and observe the correct behavior.