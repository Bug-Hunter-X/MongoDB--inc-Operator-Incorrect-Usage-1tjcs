# MongoDB $inc Operator Incorrect Usage
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field by a specified value.  However, providing a string value instead of a number will result in unexpected behavior and potentially data corruption.

## Bug
The `bug.js` file shows an example of the incorrect usage.  The `$inc` operator is used with a string value ('1'), which will not increment the counter correctly.  Instead, it will likely add the string '1' to the existing counter value (causing type conversion issues). 

## Solution
The `bugSolution.js` file demonstrates the correct usage of the `$inc` operator. The value used to increment the counter is now an integer (1), ensuring the correct behavior of the operation.
