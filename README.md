# Unhandled Error in Express.js Route Handler

This repository demonstrates a common error in Express.js applications: failing to handle potential errors within route handlers.  Specifically, this example shows a route that fetches a user by ID but lacks proper error handling for cases where the user ID is invalid or the user does not exist.

## Bug

The `bug.js` file contains the buggy code. The route handler does not check if a user exists before attempting to access user data. This can lead to application crashes or unexpected errors.

## Solution

The `bugSolution.js` file provides a corrected version.  It includes error handling to check for the existence of the user and return an appropriate response if the user is not found.

## How to run the examples

1. Clone this repository.
2. Install dependencies: `npm install express`
3. Run the buggy code: `node bug.js`
4. Run the corrected code: `node bugSolution.js`
