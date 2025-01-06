# Unhandled Exception in Asynchronous Network Request

This repository demonstrates a common error in Dart: the improper handling of exceptions during asynchronous network requests. The `bug.dart` file shows code that fetches data but doesn't adequately handle potential errors.  The `bugSolution.dart` file provides an improved version with better error handling.

## Problem

The original code uses a `try-catch` block but rethrows the exception (`rethrow;`).  If this exception isn't caught higher up in the call stack, it could lead to app crashes or unexpected behavior.  A more robust solution is needed. 

## Solution

The solution involves improving the exception handling to provide more informative error messages and to avoid propagating unhandled exceptions. Consider using more specific exception types or a custom exception class for better error management.