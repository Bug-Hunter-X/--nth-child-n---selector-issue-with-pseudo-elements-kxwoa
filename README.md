# :nth-child(n) selector issue with pseudo-elements

This repository demonstrates a common but often overlooked issue with the CSS `:nth-child(n)` selector when used in conjunction with pseudo-elements like `::before` and `::after`. The selector targets the nth child *element* of the parent, not the nth pseudo-element.

## Bug Description
The `bug.css` file contains CSS code that attempts to style pseudo-elements using `:nth-child(n)`.  However, this approach fails to produce the desired result because `:nth-child(n)` is applied to the actual child elements, not the generated pseudo-elements.

## Solution
The `bugSolution.css` file provides a solution using different techniques to achieve the same styling effect on pseudo-elements, such as directly addressing the pseudo-element with a more appropriate selector.