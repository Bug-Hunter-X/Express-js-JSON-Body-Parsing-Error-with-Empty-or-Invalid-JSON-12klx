# Express.js JSON Body Parsing Error
This repository demonstrates a common error encountered when using Express.js to parse JSON request bodies.  The issue arises when the request body is either empty or contains invalid JSON data.  The server fails to parse the body correctly, leading to unexpected behavior or errors.

## Problem
The provided Express.js server uses `express.json()` middleware to parse incoming JSON data. However, it does not handle cases where the request body is empty or contains malformed JSON. This results in an empty `req.body` or an error.

## Solution
The solution involves adding error handling to gracefully manage these scenarios.  The improved code verifies if `req.body` is empty and provides appropriate responses.
