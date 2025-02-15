# Uncommon HTML Error: Asynchronous DOM Manipulation

This repository demonstrates a common yet subtle error in HTML/JavaScript: attempting to manipulate the DOM (Document Object Model) before the elements have fully loaded.

## The Bug

The `bug.html` file contains a script that attempts to modify the `innerHTML` of a div element (`myDiv`) before the browser has finished parsing and rendering the HTML. This results in a `ReferenceError: myDiv is not defined`.

## The Solution

The `bugSolution.html` file demonstrates the solution: using the `DOMContentLoaded` event listener.  This ensures that the script executes only after the entire HTML document is parsed, preventing the error.