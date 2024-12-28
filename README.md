# Unhandled Promise Rejection in Express.js
This repository demonstrates a common error in Express.js applications: unhandled promise rejections.  Asynchronous operations, if they fail, can cause the application to crash silently, making debugging difficult.

## Problem
The `bug.js` file showcases an Express.js server with an asynchronous operation (`someAsyncOperation`). If this operation fails, the error is not caught, leading to a silent failure.  This means the server may appear to function, but it's not handling errors correctly.

## Solution
The `bugSolution.js` file shows how to correctly handle errors using a `catch` block within the asynchronous operation's promise chain. This prevents silent failures and allows for proper error handling and logging.