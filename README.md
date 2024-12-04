# Incorrect innerHTML Usage in HTML

This repository demonstrates a common, yet subtle error when using `innerHTML` to modify HTML content.  Improper usage can lead to unexpected behavior and security risks.

## Bug Description
The `bug.html` file showcases the incorrect usage of `innerHTML +=` to add a new element. This approach can unintentionally overwrite or remove existing elements within the parent container.

## Solution
The `bugSolution.html` file provides the correct approach.  Instead of directly manipulating `innerHTML`, the solution creates new elements using `createElement` and appends them using `appendChild`. This ensures better control and prevents unintended consequences.

## Learning Points
- Always prefer `createElement` and `appendChild` over directly modifying `innerHTML` for better control and security.
- Using `innerHTML +=` is generally discouraged, as it can lead to hard-to-debug issues and potential cross-site scripting (XSS) vulnerabilities.