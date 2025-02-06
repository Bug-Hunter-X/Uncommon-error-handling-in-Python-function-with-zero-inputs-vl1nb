# Uncommon Error Handling in Python Function

This repository demonstrates an uncommon error scenario in Python involving a function that handles division. The function has unexpected behavior when both input arguments are zero, resulting in a potentially misleading return value.

The `bug.py` file contains the original function with the error. The `bugSolution.py` file provides a corrected version with improved error handling.

## The Bug

The issue lies in the `function_with_uncommon_error` function. It aims to return either `a`, `b`, or `a / b` depending on the input values.  However, when both `a` and `b` are zero, it doesn't explicitly handle the `ZeroDivisionError` and returns `0` instead of raising an exception, which could mask the true underlying issue.

## The Solution

The corrected version in `bugSolution.py` addresses this by explicitly checking for the case where both inputs are zero and raising a more informative exception.