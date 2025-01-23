# CSS Specificity Issue

This repository demonstrates a subtle CSS specificity issue that can lead to unexpected styling behavior.  The problem arises from the way CSS selectors are evaluated and their inherent precedence rules.

## The Problem

The `bug.css` file contains CSS rules that define the color of paragraph elements (`<p>`) within a `div` container.  The expectation is that a paragraph within a `div` with the class `container` would have its color determined by the more specific selector.

However, due to the nature of CSS selector specificity, the less specific selector might unexpectedly win, resulting in incorrect styling.

## The Solution

The `solution.css` file demonstrates a corrected approach to style the paragraph, ensuring that the correct style is applied based on the more specific class selector. This might involve using more specific selectors or adjusting the order of the CSS rules.  Read the comments within the file for explanation.

## How to reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the unexpected color of the text.
4. Replace `bug.css` with `solution.css`.
5. Observe that the text now has the expected color.