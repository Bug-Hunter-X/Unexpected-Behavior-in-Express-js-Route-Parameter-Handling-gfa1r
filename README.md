# Unexpected Behavior in Express.js Route Parameter Handling

This repository demonstrates a common error in Express.js route parameter handling and provides a solution.

## Bug Description

Incorrectly handling route parameters in Express.js can lead to unexpected behavior, such as incorrect data retrieval or security vulnerabilities.  The bug example shows a missing check for the existence of a user, potentially leading to unhandled errors or unexpected responses. 

## Bug

The `bug.js` file contains the buggy code.  The route `/users/:id` attempts to fetch a user based on the ID. If the user doesn't exist, there is no proper handling of the `user` being `null` or `undefined`.  This can lead to errors or unexpected responses.

## Solution

The `bugSolution.js` file provides a corrected version.  It checks explicitly for the existence of the `user` before sending a response.  This ensures the application responds appropriately when a user is not found.