# Uncommon HTML Bug: Element Flashing Before Hiding

This repository demonstrates an uncommon bug in HTML where an element intended to be hidden initially briefly flashes before disappearing.  The issue stems from incorrectly using `display: none` in JavaScript to hide the element. While `display: none` removes the element from the layout, the browser may still render it briefly before the JavaScript takes effect, causing a visual flash.

## Bug Description

The `bug.html` file shows the problematic code.  A `div` is initially hidden using `display: none` in JavaScript. A `setTimeout` function later makes the `div` visible.  The element will briefly flash before being properly hidden.