# Uncommon HTML Error: innerHTML with Non-String

This repository demonstrates an uncommon error in HTML related to the usage of `innerHTML` with a non-string value.  The code attempts to assign a number directly to `innerHTML`, resulting in unexpected behavior.

## Bug Description

The `innerHTML` property expects a string value. Assigning a number directly to `innerHTML` results in the number being treated as if it were a string, but it does not render correctly in the browser. It usually leaves the element empty.  This might not raise an error, making it less detectable than other more common errors.

## Bug Solution

The solution involves explicitly converting the numerical value to a string before assigning it to `innerHTML` using the `toString()` method or string concatenation.

## How to Reproduce the Bug

1. Clone this repository.
2. Open the `bug.html` file in your web browser. 
3. Observe that the div with the id "myDiv" remains empty despite the assignment.

## How to Fix the Bug

1. Examine the `bugSolution.html` file for the corrected code.
2. Notice the use of the `toString()` method or string concatenation to ensure a string is passed to `innerHTML`.