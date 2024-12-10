# Unexpected Closure Behavior in setTimeout Loop

This repository demonstrates a common JavaScript error related to closures and the `setTimeout` function within loops.  The issue arises because the variable `i` is not captured correctly for each iteration of the loop. Instead, it's captured only after the loop completes. This leads to all the `setTimeout` callbacks logging the final value of `i` (which is 10). 

The `bug.js` file shows the problematic code.  The `bugSolution.js` file offers a corrected version, illustrating how to use `let` and immediately invoked function expressions (IIFEs) to correctly capture the value of `i` for each iteration.

This example is useful for understanding how closures work and how to avoid unexpected behavior when using `setTimeout` or `setInterval` within loops.