# Unexpected NaN Result in Javascript function
This repository contains a simple Javascript program that demonstrates an unexpected NaN (Not a Number) result when using string and numbers as function input parameters. The bug is related to the implicit type coercion in Javascript, and the solution involves explicit type checking and conversion to handle different data types effectively.

## Bug Description
The `bar` function calls the `foo` function, which performs addition. When numbers are passed to `bar`, it works as expected. However, when a string ("2") and a number (3) are passed, the `foo` function performs string concatenation instead of numerical addition. This leads to a string ("23") being returned by `foo`. The `bar` function then multiplies this string by 2, resulting in NaN.

## Solution
The solution involves explicit type checking and conversion to handle different data types gracefully. The `bugSolution.js` file contains code that addresses this issue and provides a correct implementation.