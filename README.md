# CSS calc() Issue with Percentages in Media Queries

This repository demonstrates a bug related to the CSS `calc()` function when used with percentage values inside media queries.  The expected behavior is for the width of the `.element` class to be 50% of its parent's width minus 20px. However, due to a potential misinterpretation of the percentage value within the media query context, the layout does not behave as expected.

## Bug Description

The `calc()` function doesn't correctly interpret percentage values when nested inside media queries. This leads to inconsistencies in layout across different screen sizes.

## Solution

The provided solution demonstrates a workaround that addresses the issue.  This typically involves either avoiding `calc()` within media queries or using alternative approaches such as using viewport units (`vw`) for more reliable width calculations. The solution file (bugSolution.css) offers a corrected implementation that ensures the desired width calculation behaves as intended across all screen sizes.