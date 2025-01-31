# Express.js Route Parameter Handling: 404 Error

This repository demonstrates a common error in Express.js route parameter handling and its solution. The original code lacks proper error handling when a requested user ID does not exist in the database.  The improved version demonstrates how to gracefully handle this scenario by returning a 404 Not Found response.

## Bug

The `bug.js` file contains the buggy code. It attempts to fetch user details based on an ID passed as a route parameter. If the user is not found, it will either crash or produce unexpected output. The error handling is incomplete.

## Solution

The `bugSolution.js` file provides a corrected version of the code. It explicitly checks for the existence of the user before sending the response. If the user is not found, it returns a 404 status code along with an appropriate message.