# JavaScript Hoisting Surprise!

This repo demonstrates a common but subtle issue in JavaScript related to hoisting.  The code in `bug.js` shows how accessing a variable before it's declared using `var` leads to `undefined` being printed, not an error, due to JavaScript's hoisting behavior.  The solution in `bugSolution.js` corrects this.

**Problem:** JavaScript hoists variable declarations, but not their assignments.  This means the declaration is moved to the top of the scope, but the value remains uninitialized until the assignment line is reached.

**Solution:** Declare and initialize variables before using them to avoid unexpected behavior and maintain code clarity.