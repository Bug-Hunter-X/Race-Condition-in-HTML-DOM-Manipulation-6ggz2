# Race Condition in HTML DOM Manipulation

This repository demonstrates an uncommon bug related to race conditions in HTML when manipulating the DOM using Javascript. The bug occurs when Javascript code attempts to access and modify elements before the browser has fully rendered them causing unexpected behavior or errors.

## Bug Description
The bug lies in attempting to access and modify the `innerHTML` of a `div` element before the browser has fully parsed the HTML.  This can lead to the code either failing silently or producing unexpected results.

## Solution
The solution involves using an event listener (such as `DOMContentLoaded`) or a `setTimeout` function to ensure the code executes after the DOM is fully parsed.