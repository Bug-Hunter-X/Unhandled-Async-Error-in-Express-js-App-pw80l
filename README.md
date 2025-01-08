# Unhandled Async Error in Express.js App

This repository demonstrates a common error in Node.js applications: unhandled exceptions within asynchronous callbacks.  The `bug.js` file contains an Express.js app that simulates an asynchronous operation.  Sometimes it succeeds, and other times it throws an error.  The problem is that the error isn't properly handled, leading to the application crashing without a clear indication of the problem.

The `bugSolution.js` file provides a solution using `try...catch` blocks within the async callback or promise `.catch()` to gracefully handle exceptions.