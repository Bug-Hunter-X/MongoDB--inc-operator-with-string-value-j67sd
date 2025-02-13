# MongoDB $inc operator with string value
This example demonstrates an uncommon error that occurs when using the MongoDB $inc operator with a string value instead of a numeric value.  The $inc operator is used to increment a numeric field by a given value. Using a string value leads to an unexpected outcome or an error.

## Bug
The provided code attempts to increment the `age` field by "1" (a string), resulting in a failed update operation.  The expected outcome is that the `age` field should increment by 1.  However, the current implementation results in an error or no update.

## Solution
The solution involves ensuring that the increment value provided to the $inc operator is a number.  The corrected code provides the correct usage of the $inc operator.