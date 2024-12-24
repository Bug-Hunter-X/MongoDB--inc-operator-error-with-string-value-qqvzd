# MongoDB $inc operator error with string value
This repository demonstrates an error that occurs when using the MongoDB `$inc` operator with a string value instead of a number.  The `$inc` operator is designed to increment a numerical field by a specified value. Attempting to use it with a string results in an error or unexpected behavior.

## Bug Description
The provided code incorrectly uses the `$inc` operator in a MongoDB update operation. The value being incremented is passed as a string ('1') instead of a number (1). This leads to an error or unintended result, depending on the specific MongoDB version and configuration.

## Solution
The solution involves correcting the data type of the value being incremented. The string '1' needs to be changed to the number 1. This change ensures the correct increment operation is performed by the `$inc` operator.