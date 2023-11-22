# C-Calculator

## Description:

Calculator translated from x86 Assembly to C with some added functions.

## Functionality:

* **And**: returns a signed 8 byte integer that is the bitwise AND of two 8 byte signed integers x and y
* **Or**: returns a signed 8 byte integer that is the bitwise OR of two 8 byte signed integers x and y
* **Sum**: takes in two 8 byte signed integers x and y. Updates the global variable SUM_POSITIVE and SUM_NEGATIVE depending on the sign of y.  Returns x + y
* **Array**: takes in 1) the current running result value cres, 2) the length of an array of 8 byte signed values, 3) a pointer to the beginning of the array of 8 byte signed values and 4) a pointer to a function to be called on the running result and each of the array elements. Each function is expected to return an updated running result value.  The function returns the final updated version of the running result after the array iteration.
