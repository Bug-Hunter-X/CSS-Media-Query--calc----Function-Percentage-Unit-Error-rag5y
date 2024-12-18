# CSS Media Query `calc()` Function Percentage Unit Error

This repository demonstrates an uncommon error in CSS related to the use of the `calc()` function within media queries, specifically when working with percentages without explicitly defining their reference (like viewport width or height).

## Problem
The `calc()` function in CSS is powerful but can cause unexpected behavior when used improperly with percentages.  If percentages inside `calc()` aren't referenced to a dimension like `vw` or `vh`, some browsers might misinterpret the calculation.

## Solution
Always ensure that percentages inside `calc()` within media queries are clearly tied to a viewport dimension (e.g., `vw` or `vh`) to avoid ambiguity and ensure consistent behavior across different browsers and devices. 

## Files
* `bug.css`: Demonstrates the erroneous CSS code.
* `bugSolution.css`: Shows the corrected code with units explicitly added to percentages.