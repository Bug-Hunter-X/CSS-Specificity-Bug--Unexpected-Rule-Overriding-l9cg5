# CSS Specificity Bug: Unexpected Rule Overriding

This repository demonstrates an uncommon bug related to CSS specificity.  The bug highlights a situation where multiple selectors with the same specificity target the same element, leading to unexpected overriding behavior.

## The Bug

The `bug.css` file contains CSS code that exhibits the unexpected overriding.  The fourth rule, despite seeming to have higher precedence, does not actually override the third rule due to their identical specificity. This is because they have the same number of ID, class, and element selectors.   The last rule does however override because it has an additional class selector which increases specificity.

## The Solution

The `bugSolution.css` file provides a solution to this issue. This solution highlights best practices for resolving these conflicts using more specific selectors or the important rule where appropriate.