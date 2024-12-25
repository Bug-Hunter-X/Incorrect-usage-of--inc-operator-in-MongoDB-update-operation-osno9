# Incorrect Usage of $inc Operator in MongoDB Update Operation
This example demonstrates an incorrect usage of the `$inc` operator in a MongoDB update operation.  The `$inc` operator is used to increment a numerical field by a specified value. However, attempting to increment with a string value will result in an error.

## Bug
The bug lies in passing a string value ("1") to the `$inc` operator. This will cause a MongoDB error because the operator expects a numerical value.

## Solution
The solution involves ensuring that the value passed to the `$inc` operator is a number (integer or float).
