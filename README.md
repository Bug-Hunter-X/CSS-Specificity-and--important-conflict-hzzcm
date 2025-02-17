# CSS Specificity and !important Conflict

This repository demonstrates an uncommon CSS bug related to the interaction between specificity and the `!important` declaration.  The bug highlights a scenario where a highly specific selector is unexpectedly overridden by a less specific selector due to the use of `!important`.

## Bug Description

A `!important` declaration in a less specific CSS rule can override rules with higher specificity. This behavior can be unexpected and lead to difficult-to-debug styling issues.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` and observe the CSS rules.
3. Create an HTML file to test the styles (example provided in `index.html`).
4. Observe the text color – it will be unexpectedly red instead of green. 

## Solution

The solution involves refactoring the CSS to avoid the need for `!important`, using more appropriate selectors and a structured approach to manage CSS styling.

See the corrected CSS in `bugSolution.css` for a demonstration of how to solve this issue.  The use of `!important` should be minimized for better maintainability and predictability.