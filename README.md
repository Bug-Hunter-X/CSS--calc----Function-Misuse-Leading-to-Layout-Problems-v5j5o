# CSS `calc()` Function Misuse Leading to Layout Problems

This repository demonstrates a common error involving the CSS `calc()` function.  Incorrect usage of `calc()` can lead to unexpected layout behavior, especially within flexbox containers or when dealing with percentages and fixed values.

## Bug Description

The `bug.css` file contains CSS that attempts to calculate a width based on `calc(100% - 10px)`.  However, the parent element's width is not explicitly set, leading to unpredictable results depending on the browser's interpretation of available space.

## Solution

The `bugSolution.css` file demonstrates a corrected approach. To reliably use `calc()`, ensure the parent element has a defined width (either explicitly or implicitly via constraints).