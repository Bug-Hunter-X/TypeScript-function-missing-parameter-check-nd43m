# TypeScript Function Parameter Handling Bug

This repository demonstrates a bug in a TypeScript function that doesn't properly handle optional parameters and missing required parameters.

## Bug Description

The `calculateArea` function calculates the area of a rectangle or triangle.  The `height` parameter is optional for rectangles. However, the function does not correctly handle the case where `height` is missing when calculating the area of a rectangle, resulting in a runtime error. Additionally, it handles missing parameters gracefully for unsupported shapes.

## Solution

The solution involves adding a check for the presence of the required parameters, ensuring that necessary values are always available before performing calculations.  This improvement prevents unexpected runtime errors.

## How to reproduce the bug

1. Clone the repository.
2. Navigate to the repository directory.
3. Compile and run the `bug.ts` file using a TypeScript compiler.
4. Observe the error message when calling calculateArea with an unsupported shape, missing height parameter, or invalid parameters.

## How to test the solution

1. Clone the repository.
2. Navigate to the repository directory.
3. Compile and run the `bugSolution.ts` file using a TypeScript compiler.
4. Verify that the corrected function now appropriately handles missing or incorrect parameters.