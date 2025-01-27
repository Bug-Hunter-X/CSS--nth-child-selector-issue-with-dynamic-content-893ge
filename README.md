# CSS :nth-child selector issue with dynamic content
This repository demonstrates a common issue with the CSS `:nth-child` selector when dealing with dynamically added or removed elements.  The `bug.css` file shows the problematic code, while `solution.css` provides a corrected approach.

## Problem
The `:nth-child(n)` selector can produce unexpected results if the DOM structure changes after the page's initial load.  Dynamically adding or deleting elements will alter the index calculation, causing the selector to potentially target incorrect elements.

## Solution
Using JavaScript to update the CSS styles after the DOM updates would be a better solution than relying solely on `:nth-child` in this case.