# Uncommon HTML Bug: Incorrect usage of innerText

This repository demonstrates a common yet subtle bug in HTML related to the incorrect usage of the `innerText` property.  The issue arises when attempting to set HTML content using `innerText` instead of `innerHTML`.

## Bug Description
The `innerText` property sets or gets the textual content of an element.  However, if you try to set HTML content directly using `innerText`, the browser will treat the input as plain text and escape the HTML tags.  This leads to unexpected results and can be difficult to debug.

## Bug Solution
The correct approach is to use the `innerHTML` property when you want to set HTML content.

## How to Reproduce
1. Open `bug.html` in your browser.
2. Observe that the content of the div is not updated as expected.
3. Open `bugSolution.html` to see the corrected code.