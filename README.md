# Incorrect Usage of $inc Operator in MongoDB Update Operation
This example demonstrates an error that may occur when using the `$inc` operator in MongoDB update operations. The `$inc` operator is designed to increment a numeric field by a specified value.  Attempting to increment a field with a non-numeric value will lead to an error.

## Bug
The bug involves using a string value ("1") as the increment value in the `$inc` operator. This causes the update to fail.  The correct approach is to use a numeric value.

## Solution
The solution is to ensure that the value provided to the `$inc` operator is a number (integer or float).