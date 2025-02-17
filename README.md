# MongoDB $inc Operator Error: Using String Instead of Number
This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The `$inc` operator is used to increment a numeric field by a given value.  However, if you provide a string value instead of a number, the update will fail unexpectedly.

## Bug Description
The bug arises from providing a string value ('1') to the `$inc` operator instead of a numeric value (1). This results in an incorrect update, or potentially an error. 

## Solution
The solution is simple: Ensure that the value you provide to the `$inc` operator is a number (integer or floating point) and not a string. 

## How to reproduce the bug and solution 
1. Clone this repository
2. Execute `bug.js` - This script demonstrates the incorrect usage and subsequent error.
3. Execute `bugSolution.js` - This script demonstrates the correct usage of the `$inc` operator.