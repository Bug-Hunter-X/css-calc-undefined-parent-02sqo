# CSS calc() Gotcha: Undefined Parent Width

This repository demonstrates a subtle issue that can arise when using the `calc()` function in CSS, specifically when dealing with percentage values and undefined parent widths.

## The Problem

The `calc()` function is powerful, but it relies on the context of its parent element. If you're using percentages within `calc()` and the parent element does not have an explicitly defined width, the calculation may not work as expected. This can lead to unexpected layout behavior or styling inconsistencies. 

The example in `bug.css` illustrates this problem.

## The Solution

The solution lies in ensuring the parent element has a defined width, either through setting it directly or inheriting it from its ancestor. The corrected code is shown in `bugSolution.css`.