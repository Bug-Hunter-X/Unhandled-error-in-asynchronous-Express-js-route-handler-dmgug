# Unhandled Error in Asynchronous Express.js Route

This repository demonstrates a common error in Node.js Express.js applications: unhandled errors within asynchronous route handlers.  When an error occurs in the asynchronous callback, the server will crash without proper error handling.

The `bug.js` file shows the problematic code.  The `bugSolution.js` file provides a solution using `try...catch` blocks or error-handling middleware to gracefully handle these scenarios.

## How to reproduce the bug:

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `node bug.js`. The server will start.
4. Make multiple requests to `http://localhost:3000/`.  Eventually, the server will crash due to an unhandled error.