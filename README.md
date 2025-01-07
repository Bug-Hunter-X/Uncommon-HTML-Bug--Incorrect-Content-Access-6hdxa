# Uncommon HTML Bug: Incorrect Content Access

This repository demonstrates a common yet easily overlooked mistake when working with HTML content:  incorrectly accessing the content of an HTML element.  The bug focuses on the difference between `textContent` and `innerHTML`.

## The Bug

The `bug.html` file contains a simple HTML structure with a `<div>` element containing some text.  A JavaScript snippet attempts to access the content of the div.  However, it uses `textContent` when the intention might be to get the entire HTML markup including the `<p>` tag and other possible nested tags, for which `innerHTML` would be appropriate.

## The Solution

The `bugSolution.html` file shows the corrected approach using `innerHTML` to retrieve the complete HTML content of the div, including any nested tags and their attributes. This solution resolves the potential issue for many situations where the intention is not merely to get the text only, but rather the complete HTML structure within a specific element.

## How to run

1. Clone this repository.
2. Open `bug.html` and `bugSolution.html` in a web browser.
3. Open the browser's developer console (usually by pressing F12) to view the output from the JavaScript code.