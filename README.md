# C-Calculator

## Description:

Calculator translated from x86 Assembly to C with some added functions.

## Functionality:

* **And**: returns a signed 8 byte integer that is the bitwise AND of two 8 byte signed integers x and y
* **Or**: returns a signed 8 byte integer that is the bitwise OR of two 8 byte signed integers x and y
* **Sum**: takes in two 8 byte signed integers x and y. Updates the global variable SUM_POSITIVE and SUM_NEGATIVE depending on the sign of y.  Returns x + y
* **Array**: takes in 1) the current running result value cres, 2) the length of an array of 8 byte signed values, 3) a pointer to the beginning of the array of 8 byte signed values and 4) a pointer to a function to be called on the running result and each of the array elements. Each function is expected to return an updated running result value.  The function returns the final updated version of the running result after the array iteration.
* **Array Sum**: takes in 1) the current running result 2) the length of an array of 8 byte signed integers, and 3) a pointer to the beginning of the array of 8 byte signed integers.  This function calls the csum function to each element and updates the running result as it goes.  The function returns the final updated running result value.
* **List**: takes in 1) the running result, 2) an address of where the beginning of a list (head) and 3) a pointer to a function to call on the running result and each element of the list.  clist returns the final running result.
* **List Sum**: like arraysum but works on a list of elements
* **Upper**: takes in 1) running result and 2) a pointer to an ascii string. The function should upper case any lower case characters in the string and return the addition of the string length to the running result.
* **Atoq**: Takes in 1) the current running result and 2) add a pointer to an ascii string.  It should attempt to decode and ascii integer from the beginning of the string into an 8 byte signed value and then call the csum function on the running result and the decoded value updating the running result.
