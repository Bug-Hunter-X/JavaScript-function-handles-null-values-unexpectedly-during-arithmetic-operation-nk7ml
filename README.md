# JavaScript Null Handling Bug

This repository demonstrates a common bug in JavaScript related to null handling in functions performing arithmetic operations. The `foo` function is expected to add two numbers, but it returns `null` when either or both inputs are `null`. This might not be the expected behavior in all scenarios, potentially leading to unexpected results or errors in applications.

## Bug Description

The issue lies in the function's handling of `null` values. Instead of providing a more robust handling mechanism (like defaulting to 0 or throwing an error), it simply returns `null`. This can lead to unexpected outcomes when `null` values are part of the input data.

## Solution

A better approach would be to check for `null` values and handle them accordingly. For example, the function could treat `null` as 0, or it could throw an error to indicate that a null value is not allowed.