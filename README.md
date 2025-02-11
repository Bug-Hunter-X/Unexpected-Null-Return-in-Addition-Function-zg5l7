# Unexpected Null Return in Addition Function

This repository demonstrates a subtle bug in a JavaScript function that handles null values unexpectedly.  The `foo` function is intended to add two numbers. However, it returns `null` if either of the input arguments is `null`, even if the other argument is a valid number. This behavior might not be what's expected in all cases.

The `bug.js` file contains the buggy code.  The `bugSolution.js` file provides a corrected version.

## Bug Description

The `foo` function immediately returns `null` if either input is null, instead of handling the null value appropriately.  This might lead to unexpected results and potential errors if the function is used in a context where null values might be present but shouldn't result in an immediate `null` return. 