# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript pitfall: unexpected behavior when using loose equality (==) to compare null and undefined values. The bug arises from the fact that while both null and undefined are falsy, they are not considered strictly equal using the loose equality operator.  The provided solution demonstrates how to avoid this error and write more robust code.

## Bug Description

The provided code uses loose equality to check if a value is null. However, due to the loose comparison rules of ==, it fails to produce consistent results with undefined. This leads to unexpected NaN outputs when the function receives undefined as input. 

## Solution

The solution uses strict equality (===) to solve this. Strict equality compares both the value and type, so it more reliably checks whether a value is exactly null.